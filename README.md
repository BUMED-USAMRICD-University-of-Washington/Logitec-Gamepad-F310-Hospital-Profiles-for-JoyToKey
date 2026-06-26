# Logitech Gamepad F310 - Clinical & Hospital Workstation Profiles for JoyToKey

This repository contains a curated ecosystem of highly optimized, precision-tuned JoyToKey (`.cfg`) configuration profiles for the **Logitech Gamepad F310** controller. These profiles map complex keyboard and mouse multi-key shortcut combinations natively found inside high-density medical imaging platforms, clinical dental practice management frameworks, surgical planning applications, and video management infrastructure to the gamepad interface.


**Code written by Fleet Admiral Correo "MIRICYL BABY" Hofstad - USN,** ***The U.S. Navy SEAL who coded the XBOX controller for the Submarine Service.***
 1. https://www.navy.mil/Press-Office/Press-Releases/display-pressreleases/Article/2247544/uss-colorado-commissioned/
 2. https://apps.dtic.mil/sti/tr/pdf/AD1088622.pdf


## ⚠️ Clinical Production Environment Disclaimer
Standard commercial gaming controllers and macro mapping utility layers (like the Logitech F310 and JoyToKey) lack medical-grade physical isolation barriers, real-time hardware fail-safe redundancy loops, and haptic error feedback modules. 
* **Scope of Use:** These configurations are tailored strictly for clinical workstation planning, diagnostic image post-processing review, data navigation, student education, and prototyping environments. 
* **Caution:** They are not engineered for, nor to execute, the real-time movement manipulation of live human surgical robotics or active therapeutic interventions.

---


## 📈 System Components & Procurement Routing

| Hardware Node | System Operational Purpose | Strategic Marketplace Access |
| :--- | :--- | :--- |
| **Logitech Gamepad F310** | High-stiffness, zero-drift analog translation interface featuring dual-bumper chorded multi-mapping layers. | [Secure Primary Controller](https://amzn.to/3T3mLam) |
| **USBGear 4-Port Hub** | Mountable, metal-enclosed USB 3.2 Gen 1 SuperSpeed backplane ensuring completely isolated 5Gbps device communication data tracks. | [Secure Communication Backplane](https://amzn.to/3R5Er4H) |

---

## 🛠️ Hardware Setup: Mandatory DirectInput Toggle
Before launching your workstation or loading any configuration profiles into the JoyToKey application layer, look at the physical rear housing of your **Logitech Gamepad F310**. 
1. Locate the slide toggle switch labeled **X** (XInput) and **D** (DirectInput).
2. Firmly click the switch over to the **D** position (**DirectInput mode**).
3. Connect the controller via USB to the host workstation.

*DirectInput mode is required for JoyToKey to properly isolate and interpret the analog triggers (`LT` / `RT`) as digital threshold switches and cleanly shift between chorded multi-mapping layers.*

---

## 🔬 Precision Sensitivity & Calibration Framework

To protect alignment workflows and ensure sub-millimeter cursor selection accuracy on high-density 4K medical display cockpit matrices, every profile in this repository implements strict, hardware-level filtering rules:

* **Stiff Dead Zones (`StickDeadZone=18` to `20`):** Commercial joysticks carry physical slack near their resting center. Enforcing a deep dead zone completely filters out mechanical play and physical hand vibrations. The pointer will remain stable even when a hand rests on the joystick.
* **Dampened Exponential Velocity Curve (`Axis1X=1, -32`):** Rather than standard linear tracking speed, stick input values are heavily scaled down. Subtle thumb shifts translate to tiny sub-voxel adjustments on the screen, while pushing the stick fully to the edge allows for faster navigation across multi-display walls.
* **Analog Trigger Threshold Switches (`, 75` to `, 85`):** The lower analog levers (`LT`/`RT`) function as gradual sliders in DirectInput. These files add explicit compression percentage thresholds. A parameter change, chart save, or frame freeze will only execute upon an intentional, deep throw (e.g., 85% compressed), completely stopping accidental activation if a trigger is lightly brushed.
* **Chorded Shift Layers:** Holding down the Left Bumper (`LB` / Layer 2) or Right Bumper (`RB` / Layer 3) immediately changes the function of the face buttons (`A, B, X, Y`) and triggers, providing muscle-memory access to up to 24 separate clinical macros per profile without needing to touch a keyboard.

---

## 📂 Configuration Repository Index

### 🎥 Radiology, Imaging, & Post-Processing (PACS)
*   [`Horos_OsiriX_PACS.cfg`](./profiles/Horos_OsiriX_PACS.cfg): Optimized for rapid MRI/CT multi-slice scrolling, window/leveling, and fine ROI measurement tracing in open-source MacOS ecosystems.
*   [`TeraRecon_Intuition_Clinical.cfg`](./profiles/TeraRecon_Intuition_Clinical.cfg): Maps advanced centerline tracking tools, CPR views, automated lumen sizing arrays, and MIP/VRT layout configurations.
*   [`Canon_Medical_Vitrea_Clinical.cfg`](./profiles/Canon_Medical_Vitrea_Clinical.cfg): Features instant access to organ segmentation pipelines, Hounsfield Unit maps, multi-planar reconstruction alignment views, and calcium scoring arrays.
*   [`Siemens_SyngoVia_Clinical.cfg`](./profiles/Siemens_SyngoVia_Clinical.cfg): Provides chorded control over automated vascular extraction profiles, tissue threshold masks, cross-series navigation links, and syngo application tabs.
*   [`Carestream_VuePACS_Clinical_Precision.cfg`](./profiles/Carestream_VuePACS_Clinical_Precision.cfg): Dedicated Carestream environment mapping for multi-planar reconstructions, cross-series scrolling synchronization links, and targeted diagnostic window presets (Brain, Bone, Lung, Soft Tissue).

### 📐 Active Clinical Planning Workstations
*   [`3D_Slicer_Clinical_Precision.cfg`](./profiles/3D_Slicer_Clinical_Precision.cfg): Dampened layout for Slicer's Segment Editor toolset, including Paint, Erase, Threshold adjustments, Grow from Seeds, and anatomical view manipulation keys (A, P, L, R).
*   [`Brainlab_Elements_Clinical_Precision.cfg`](./profiles/Brainlab_Elements_Clinical_Precision.cfg): Tailored for cranial/spinal target contouring, establishing trajectory entry and target points, toggling DTI fiber tracking views, and triggering auto-dataset fusion locks.
*   [`Medtronic_StealthStation_Clinical_Precision.cfg`](./profiles/Medtronic_StealthStation_Clinical_Precision.cfg): High-stability profile mapping coordinate tracking frameworks, trajectory target lines, multi-planar planning matrices, and optical camera co-registration maps.
*   [`Materialise_Mimics_Clinical_Precision.cfg`](./profiles/Materialise_Mimics_Clinical_Precision.cfg): Precision setup for voxel segmentation in Mimics Medical and implant optimization tools in 3-matic. Includes Split Mask, Smart Fill, Crop Box, and 3D STL calculation triggers.
*   [`BioDigital_Human_Interactive.cfg`](./profiles/BioDigital_Human_Interactive.cfg): Fluent 3D camera orbits, structure hide/fade toggles, system layout maximize hooks, and interactive tour timeline navigation tracking.

### 🏥 Surgical Cockpit, Video Routing, & Endoscopic Camera Platforms
*   [`Stryker_Surgical_Media_Sensitivity_Tuned.cfg`](./profiles/Stryker_Surgical_Media_Sensitivity_Tuned.cfg): Supports SDC4K/Connected OR platforms. Maps still photo capture, video recording toggles, white balance execution, PIP layout routing, digital zoom tuning, and AIM/ICG visualization filter profiles.
*   [`Karl_Storz_AIDA_Sensitivity_Tuned.cfg`](./profiles/Karl_Storz_AIDA_Sensitivity_Tuned.cfg): Formatted for AIDA/IMAGE1 S ecosystems. Features quick-toggles for screen grid matrices (Single, Split, PIP, Quad), live stream freezes, and S-Technologies color gain filters (CLARA, CHROMA, SPECTRA).
*   [`Olympus_Visera_IMH_Sensitivity_Tuned.cfg`](./profiles/Olympus_Visera_IMH_Sensitivity_Tuned.cfg): Configured for EVIS X1/VISERA ELITE environments. Focuses on examination gallery navigation, auto-focus execution, and optical modality enhancements like Narrow-Band Imaging (NBI) and Near-Infrared fluorescence.

### 🦾 Interactive Clinical System Displays
*   [`Stryker_Mako_SmartRobotics_Clinical.cfg`](./profiles/Stryker_Mako_SmartRobotics_Clinical.cfg): Maps haptic boundary overlays, live bone resection depth parameters, orthopedic component sizing modifications, and varus/valgus alignment tilt vectors.
*   [`Medtronic_Hugo_RAS_Simulation.cfg`](./profiles/Medtronic_Hugo_RAS_Simulation.cfg): Handles independent modular arm cart staging profiles, open-console workspace parameters, and Rubina 3D HD fluorescence image subtraction modes.
*   [`CMRSurgical_Versius_Simulation.cfg`](./profiles/CMRSurgical_Versius_Simulation.cfg): Coordinates bedside arm profiles, v-wrist tool clearance checks, stereoscopic scope zoom increments, and structural contrast filter presets.
*   [`Globus_Medical_ExcelsiusGPS_Clinical.cfg`](./profiles/Globus_Medical_ExcelsiusGPS_Clinical.cfg): High-stiffness profile for pedicle screw length and diameter calculations, planning coordinates confirmation, and surveillance optical alignment verification arrays.
*   [`Medtronic_MazorX_Stealth_Clinical.cfg`](./profiles/Medtronic_MazorX_Stealth_Clinical.cfg): Coordinates automated spinal navigation tracking boundaries, multi-planar reconstruction views, robotic arm alignment lines, and StealthStation optical co-registration maps.
*   [`Intuitive_Ion_Endoluminal_Clinical.cfg`](./profiles/Intuitive_Ion_Endoluminal_Clinical.cfg): Tuned for peripheral lung lesion targeting. Tracks catheter alignment, virtual-to-live bronchoscopy overlays, lesion distance metrics, and optimal pathway calculations.
*   [`Intuitive_daVinci_SP_Clinical.cfg`](./profiles/Intuitive_daVinci_SP_Clinical.cfg): Structured for single-cannula instrument arm staging, triangulation workspace checking, and 3DHD narrow-profile scope focal zoom increments.
*   [`JJMedTech_Monarch_Platform_Clinical.cfg`](./profiles/JJMedTech_Monarch_Platform_Clinical.cfg): Optimized for electromagnetic guidance logs, peripheral airway pathing, target node placement, and live endoluminal video overlays.

### ⚡ Interventional Therapy & Hybrid Suites
*   [`Philips_Azurion_FlexVision_Clinical.cfg`](./profiles/Philips_Azurion_FlexVision_Clinical.cfg): Navigates FlexVision Pro display walls, stepping frame-by-frame through DSA cine runs, and managing real-time Roadmap overlays and ClarityIQ noise reduction filters.
*   [`Siemens_Artis_Icono_Pheno_Clinical.cfg`](./profiles/Siemens_Artis_Icono_Pheno_Clinical.cfg): Connects syngo workflow tiles, enabling multi-planar window contrast alterations, subtraction masks, and CLEARstent live stent optimization views.
*   [`GE_HealthCare_Allia_Innova_Clinical.cfg`](./profiles/GE_HealthCare_Allia_Innova_Clinical.cfg): Interoperable layout for Central Touch Panels (TPM), controlling Innova3D volumetric reconstructions, VesselAssure vectors, and ValveASSIST heart overlays.
*   [`GE_HealthCare_Allia_Innova_Clinical.cfg`: Interoperable layout for Central Touch Panels (TPM), controlling Innova3D volumetric reconstructions, VesselAssure vectors, and ValveASSIST heart overlays.
*   [`Canon_Alphenix_4DCT_Hybrid.cfg`: High-stakes hybrid layout managing Aquilion CT volume stacks, Alphenix angio runs, embolization planning paths, and Illuxtra 3D vessel tracking.

### 📐 Radiotherapy Patient Alignment, Gating, & SGRT

*   [`LAP_Laser_Apollo_Astor_Precision.cfg`: Manages room coordinate calibration files, manual laser translation adjustments, laser auto-zero routines, and multi-planar geometric measurement crosshairs.
*   [`Sun_Nuclear_Gammex_MicroPlus_Precision.cfg`: Enforces high center dead zones for daily phantom QA, step-size alterations, isocenter verification checks, and system standby transitions.
*   [`CYRPA_HIT_Laser_Precision.cfg`: Configured for moving laser arrays, allowing safe step tracking increments, phantom benchmark locks, and real-time room calibration verification.
*   [`Vision_RT_AlignRT_Clinical_Precision.cfg`: SGRT interface mapping for real-time region of interest (ROI) selection, motion gating threshold scaling, surface heat map displacements, and immediate baseline capture accept locks.
*   [`CRAD_CatalystPlus_Clinical_Precision.cfg`: Integrates live intrafraction motion trend charts, respiratory gating tolerance shifts, baseline contour overlays, and verified configuration locks.
*   [`LAP_LUNA3D_Clinical_Precision.cfg`: Connects optical camera validation monitors, providing structured control over delta positioning grids, thermal displacement maps, and verified setup parameters.

### 🦷 Dental Practice Management & Intraoral Specialists

*   [`HenryScheinOne_Dentrix_Clinical.cfg`: Dental charting environment profile featuring a dedicated Periodontal pocket-depth numerical entry mapping via chorded D-pad/Face key combinations, module routing, and radiograph contrast sharpening filters.
*   [`Carestream_Dental_CSImaging_Clinical.cfg`: Formatted for CS Imaging suites. Includes mandibular nerve canal seed mapping, 3D structure transparency toggles, implant simulation templates, and cephalometric ray tracing overlays.
*   [`Carestream_PracticeWorks_Clinical.cfg`: High-precision layout managing Appointment Books, clinical notes text input focus jumps, treatment plan fields, account ledgers, and intraoral bone grids.

### 📋 Healthcare Technology Management (HTM) & Clinical Engineering

*   [`Phoenix_Data_Systems_AIMS_Precision.cfg`: Optimized for biomedical asset registry workflows, logging labor/parts expenses, toggling work order statuses (In Progress, Waiting for Parts, Complete), and executing PM compliance checklist validations.
*   [`Nuvolo_ConnectedWorkplace_Clinical.cfg`: Formatted for Nuvolo CLM platforms on ServiceNow. Maps precise database row selections, automated parts request workflows, lifecycle state parameters, and electronic signature submittals.
*   [`MediMizer_Asset_Management_Precision.cfg`: Enforces strict dead zones for navigating dense equipment logs, managing preventive maintenance (PM) compliance profiles, and executing server validation sync updates.

### 🌐 Hospital Facilities, Building Management (BMS) & RTLS Infrastructure

*   [`CenTrak_RTLS_Clinical_Precision.cfg`: Tailored for CenTrak's clinical-level visibility systems. Maps floor-plan navigation, tracking node queries, dirty utility/clean room tag status updates, and emergency alert acknowledgments.
*   [`Securitas_AeroScout_RTLS_Precision.cfg`: High-density map navigation for AeroScout Wi-Fi asset tracking and environmental temperature monitoring. Allows rapid vaccine refrigerator temp-check logging and staff safety alert silencing.
*   [`Schneider_Electric_EcoStruxure_Healthcare.cfg`: Controls Power SCADA dashboards, environmental overlays, isolation room negative/positive pressure state flips, and airflow air changes per hour (ACH) fan tuning.
*   [`Siemens_DesigoCC_Healthcare_Precision.cfg`: Interfaces with Desigo CC systems to review medical gas pipelines, calibrate OR laminar airflow variables, manipulate graphic plant overlays, and acknowledge building infrastructure faults.

### 📋 EHR, Spreadsheet Management, & Clinical Registries

*   [`Medical_EHR_Data_Management.cfg`: A production-grade macro layout built to accelerate long XLS/CSV registries and Electronic Health Record databases (Epic, Cerner, eClinicalWorks). Bridges fast column/row sheet scrolls, global searches, clipboard hooks, row insertion/deletion filters, and e-signature chart sign-off commands.

### 📑 Clinical Laboratory & Specialized Diagnostics

*   [`LabWare_LIMS_Enterprise.cfg`: Provides chorded control over high-throughput specimen logs, plate map overlays, row filtering, and bulk batch validation sign-offs.
*   [`Natus_Otosuite_Audiology.cfg`: Maps manual hearing level decibel (dB) selections, stimulus octave frequency tracking (Hz), continuous/pulsed stimulus audio tone delivery, red/blue ear channels, and tympanometry layouts.
*   [`Philips_IntelliSpace_ICCA.cfg`: Designed for ICU and anesthesia care auditing. Scrubs historical physiological vital timeline streams (ECG, capnography, lines) continuously over hours while flagging medical intervention markers.
*   [`Zeiss_Forum_Ophthalmology.cfg`: Retinal imaging post-processing tool. Maps foveal OCT slice scroll stacks, macular thickness maps, eye comparison panels (OD vs. OS), and retinal layer tracking lines.
*   [`Varian_Eclipse_TPS.cfg`: Radiation oncology inverse treatment planning optimization. Triggers structural organ-at-risk (OAR) contour mapping, multi-angle beam targets, multi-leaf collimator (MLC) shapes, and Dose-Volume Histogram (DVH) overlays.

### 🎓 Interactive Clinical Reasoning, Simulation, & Surgical Training

*   [`Osso_VR_Proctor_Precision.cfg`: Proctor dashboard companion layout for tracking multi-user VR operating room lobbies, zooming 3D feeds, toggling tool trays, and submitting performance scorecards.
*   [`PrecisionOS_Proctor_Evaluation.cfg`: Evaluation node profile for checking biomechanical loading data, tracking bone-screw vectors, spinal alignment tolerances, and pushing certification analytics.
*   [`FundamentalVR_Proctor_Evaluation.cfg`: Connects case evaluator panels to monitor sub-surface tissue deformation scales, bone incision pathways, force feedback parameters, and multi-angle reference cameras.
*   [`BodyInteract_Clinical_Reasoning_Precision.cfg`: Instructors profile to navigate acute distress tracking timelines (cardiac arrest, trauma), manage drug orders, launch intubations, and log performance scores under time metrics.
*   [`Oxford_Medical_Simulation_OMS_Precision.cfg`: Nursing and medical school proctor system. Maps timeline logs, communication marker grids, prioritization dashboards, and diagnostic debriefing card submittals.
*   [`Laerdal_LLEAP_SimMan_Precision.cfg`: Drives the LLEAP software backbone behind robotic patient mannequins. Features quick-keys for triggering sudden hemorrhages, tongue edema, laryngospasms, cardiac arrest, and CPR quality checks.
*   [`Kenhub_Anatomy_Learning_Precision.cfg`: Accelerates learning with a multiple-choice response keypad (Options A-D), automated quiz navigation, flashcard flipping loops, and Latin/English toggle switches.
*   [`Osmosis_OnlineMedEd_BoardPrep.cfg`: Optimized for intense USMLE/NCLEX board prep. Maps HTML5 video speed scaling, timeline scrubbing arrows, Qbank checklist boxes, and playlist hooks.

* * * * *
