# Physical AI — Institutional-Grade Equity Research Report

**Author:** Internal research draft
**Date:** May 22, 2026
**Mandate:** A focused investment framework for Physical AI — robotics, embodied AI, autonomous physical systems, and industrial automation — over the next 5–10 years.
**Scope discipline:** This is not a datacenter AI report. GPUs, HBM, CoWoS, optical interconnects, and hyperscaler capex are only referenced where they materially affect physical machines that move, manipulate, inspect, or defend in the real world.

**Data caveat:** Financial figures (market caps, revenue, segment splits, margins) are best-effort and reflect roughly FY2024–FY2025 reporting unless otherwise noted. Every number that is materially uncertain is flagged with "approx." Always verify against the most recent 10-K, 20-F, or interim report before acting.

---

## A. Executive Summary — The Direct Verdict

**Is Physical AI investable today?** Yes — but *not* in the form most retail investors are pricing it.

The investable Physical AI thesis over 5–10 years is **boring industrial compounders, sensor and motion-control specialists, and the surgical-robotics monopoly** — not humanoid-robot OEMs. The visible economics today accrue overwhelmingly to:

1. **Industrial automation incumbents** (ABB, Siemens, Rockwell, Schneider, Fanuc, Yaskawa, Omron, Mitsubishi Electric). They sit at the chokepoint between any new robot fleet and the factory floors that must absorb them. They control PLCs, drives, safety, fieldbus, MES, and the integrator relationships. **They will not be disintermediated by a humanoid robot startup.**
2. **One genuine durable robotic-platform monopoly**: Intuitive Surgical (ISRG). It is the closest thing public markets have to a "buy Physical AI" stock with proven recurring revenue and 70%+ market share.
3. **Embedded compute + sensing component oligopolies** (NVIDIA Jetson/Isaac, Cognex machine vision, Analog Devices motor control, Allegro magnetic sensing, MPWR power management). These are the picks-and-shovels.
4. **Test & validation** (Keysight, Teradyne, Cognex metrology) — the unsexy gating layer between a prototype humanoid and a deployable one.

**Where economics will *not* accrue (high-conviction):**
- The vast majority of humanoid robot OEM startups. The business model — selling labor-as-a-service at price points that compete with $15/hr labor — has weak unit economics in the absence of dramatic component-cost declines. Most humanoid valuations in private markets (2023–2025 vintage at $5B–$40B pre-revenue) will not be validated by 2030.
- Lidar pure-plays except as venture-style satellites. Commoditization is faster than expected.
- Most "AI-enabled" warehouse robotics startups; the warehouse-robotics value chain is being absorbed by Symbotic (concentrated customer risk) and the incumbent material-handling players.

**The framing question** — *where do public equity investors actually make money if Physical AI becomes a major wave?* — resolves to: **motion control, sensing, embedded compute, surgical robotics, and industrial automation incumbents.** Robot OEMs are a satellite trade, not a mansion trade. Humanoid hype is the dominant retail mispricing.

The $500K Mansion Model that follows reflects this: 7 mansion positions across 6 subsectors, none of which is a pure humanoid bet, but with deliberate satellite exposure to humanoid component suppliers, defense autonomy, and lidar to capture asymmetric upside without making it the thesis.

---

## 1. Defining Physical AI

These terms are conflated routinely. The distinctions matter for capital allocation.

| Term | Definition | Where the economics live |
|---|---|---|
| **Software AI** | LLMs, vision models, copilots; runs in datacenters or on user devices. | Hyperscalers, model labs, NVIDIA datacenter. |
| **Datacenter AI** | The training and inference of large models on GPU/TPU clusters. | NVIDIA, AMD, Broadcom, TSMC, SK Hynix, hyperscalers. *Not the focus of this report.* |
| **Edge AI** | Inference on devices outside datacenters — phones, cars, cameras, robots. | Qualcomm, Ambarella, MediaTek, Hailo (private), NVIDIA Jetson, NXP. |
| **Robotics** | Mechatronic systems combining sensing, actuation, and control to perform physical tasks. May or may not contain modern AI. Includes traditional industrial robotics (1970s–present). | Fanuc, ABB, Yaskawa, KUKA (private/Midea), Mitsubishi, Kawasaki, Universal Robots (Teradyne). |
| **Embodied AI** | AI systems whose intelligence is conditioned on having a physical body — perception, action, and learning are tightly coupled. The current wave of vision-language-action (VLA) models is the technical core. | Mostly private today: Physical Intelligence, Skild AI, Covariant (now Amazon); NVIDIA's GR00T/Cosmos/Isaac stack is the dominant public-equity exposure. |
| **Autonomous physical systems** | Machines that operate without continuous human control: self-driving cars, autonomous drones, autonomous ships, autonomous mining vehicles, autonomous tractors. | Tesla, Mobileye, Aurora, Waymo (Alphabet), Anduril (private), Kratos, AeroVironment, Deere. |
| **Industrial automation** | Programmable factory infrastructure: PLCs, drives, motion control, SCADA, MES, fieldbus. Predates "AI" by decades. | Siemens, Rockwell, ABB, Schneider, Mitsubishi, Omron, Emerson. |
| **Humanoid robots** | General-purpose bipedal/anthropomorphic robots designed to operate in human-shaped environments. | Mostly private: Figure, 1X, Apptronik, Agility, Sanctuary, Unitree, Boston Dynamics (Hyundai). Public proxies: TSLA (Optimus), NVDA (compute), suppliers (HRL, Nidec, Maxon, harmonic-drive vendors).|

**Physical AI**, as used here, is the union of *embodied AI + autonomous physical systems + the modernization of industrial automation*. It is broader than humanoids and narrower than "all AI applied to physical things."

---

## 2. The Full Physical AI Stack

### A. Robot intelligence / training layer
- **Foundation models for robotics:** VLA models (vision-language-action). Public exposure: NVIDIA (GR00T, Cosmos world model, Isaac Lab). Private: Physical Intelligence (π₀, π-0.5), Skild AI, DeepMind RT-X, Covariant Brain (Amazon).
- **Sim-to-real / synthetic data:** NVIDIA Omniverse / Isaac Sim is the dominant commercial platform; ANSYS (Synopsys), Dassault Systèmes, Siemens (Tecnomatix/Process Simulate) compete on the digital-twin axis. Open source: MuJoCo (DeepMind), Drake (TRI).
- **Digital twins:** Siemens Xcelerator, Dassault 3DEXPERIENCE, PTC (Onshape/Vuforia), Bentley Systems, ANSYS, AVEVA (Schneider).
- **Fleet learning:** Largely captive (Tesla Autopilot, Waymo, Amazon Robotics). No clean public-equity expression.

**Economics:** Software + compute. The economics here look like normal SaaS plus chip sales. NVIDIA captures by far the most.

### B. Embedded compute
- **Edge / robotics SoCs:** NVIDIA Jetson (Orin, Thor in 2025), Qualcomm Robotics RB platform, Ambarella CVflow, Hailo (private), Texas Instruments TDA4.
- **Industrial MCUs:** NXP, STMicroelectronics, Renesas, Microchip, Infineon.
- **Industrial processors:** Intel (industrial Atom), AMD (Xilinx FPGAs), Microsemi (Microchip).
- **Power-efficient accelerators:** Qualcomm, Ambarella, Hailo, Mythic (private), Tenstorrent (private).

**Economics:** NVIDIA captures the high-end "robot brain" socket. Below the brain, the MCU and analog-mixed-signal players (NXP, STM, Infineon, TI, ADI) capture the broader and more numerous "limb" sockets. Per-unit dollar content from these is small but volume is structurally large and growing.

### C. Sensors and perception
- **Industrial cameras / machine vision:** Cognex, Keyence (private-feeling but listed in Japan, 6861.T), Basler, Teledyne (DALSA), Omron, Sick.
- **Lidar:** Hesai (HSAI), Ouster (OUST), Innoviz (INVZ), Luminar (LAZR), Aeva (AEVA), Valeo, Bosch (private), RoboSense.
- **Radar:** NXP, Infineon, Texas Instruments, Continental, Bosch, Aptiv.
- **Tactile / force-torque:** ATI Industrial (private, Novanta-owned partially), Robotiq (private), OnRobot (private), HEX (private).
- **IMUs:** Analog Devices (high-precision MEMS), STMicro, Bosch Sensortec, TDK-InvenSense.
- **Safety sensors / light curtains:** Sick (private), Keyence, Banner, Omron, Pilz (private), Pepperl+Fuchs (private).

**Economics:** Cognex is the cleanest pure-play with structural moats. ADI dominates high-precision MEMS IMUs. Lidar is commoditizing fast. Keyence (Japan) is the highest-quality vision company globally but trades at premium multiples and limited ADR liquidity.

### D. Actuation and motion control
- **Servo motors:** Yaskawa, Mitsubishi, Fanuc, Siemens, Rockwell (Allen-Bradley), ABB, Nidec (6594.T), Maxon (private), Moog.
- **Drives / motor controllers:** Same vendor set; Allegro (ALGM), Monolithic Power (MPWR), Texas Instruments, Infineon, ON Semi provide the silicon.
- **Harmonic reducers / precision gears:** Harmonic Drive Systems (6324.T) is the global pure-play monopoly for the strain-wave gears used in collaborative and humanoid robot joints. Nabtesco (6268.T) for RV reducers. Sumitomo, SEW-Eurodrive.
- **Motion-control software:** Beckhoff (private), Bosch Rexroth, Siemens SINUMERIK, Rockwell Logix, KEB.

**Economics:** This is the **single most underappreciated economic chokepoint** of the entire humanoid wave. A humanoid robot needs 20–40 actuator joints, each requiring a motor + reducer + drive electronics + feedback sensor. The harmonic-reducer vendors (Harmonic Drive Systems, Nabtesco) and the high-precision servo vendors (Yaskawa, Fanuc, Nidec, Maxon) are the closest thing to "you cannot build a humanoid without us." Allegro and MPWR ride on the silicon side. **This is where the report's strongest underappreciated thesis lives.**

### E. Power systems
- **Batteries:** Panasonic, Samsung SDI, LG Energy Solution, CATL (300750.SZ), BYD. For humanoids and small autonomous platforms, power density is the binding constraint on operating runtime (most humanoids today run 2–4 hours per charge).
- **Charging:** Limited public pure-play exposure outside auto-EV.
- **Power management ICs:** Monolithic Power (MPWR), Analog Devices, Texas Instruments, Infineon, ON Semi, Allegro, Vishay.
- **Motor power electronics / WBG semiconductors:** SiC and GaN are increasingly used in motor drives for efficiency. Wolfspeed (WOLF), STM, Infineon, ON Semi, Rohm. **Wolfspeed is a balance-sheet wreck and should not be confused with a clean Physical AI thesis.**

**Economics:** Power management is structurally durable. MPWR is the cleanest beneficiary because of its mixed-signal/analog DNA and motor-control penetration.

### F. Industrial networking and controls
- **PLCs:** Siemens (Simatic, ~30% global share), Rockwell (Logix, dominant in North America), Mitsubishi, ABB, Schneider, Omron.
- **Industrial Ethernet / TSN:** ProfinetIO (Siemens-led), EtherCAT (Beckhoff-led), EtherNet/IP (Rockwell-led), CC-Link IE TSN (Mitsubishi).
- **Fieldbus:** Profibus, DeviceNet, Modbus — legacy but enormous installed base.
- **Factory control / MES / SCADA:** Siemens (Opcenter), Rockwell (Plex/FactoryTalk), AVEVA (Schneider), Honeywell (Forge).

**Economics:** This is a **regulated-utility-like layer** with extraordinarily sticky installed bases. New robot OEMs MUST integrate into these protocols. Siemens and Rockwell are the most direct beneficiaries.

### G. Safety, reliability, compliance
- **Machine safety:** Pilz (private), Sick, Rockwell (Guardmaster), ABB (Jokab), Schmersal, Banner, Keyence, Omron.
- **Functional safety semis:** Infineon, NXP, TI, STM (ISO 26262 / IEC 61508 certified parts).
- **Certification bodies:** TÜV, UL (Underwriters Laboratories, private), DNV — not publicly investable.
- **Cybersecurity for OT:** Dragos (private), Claroty (private), Nozomi (private); Honeywell Forge, Siemens (acquired Foghorn / Forescout), Rockwell partnered with Dragos. CrowdStrike and Palo Alto have OT plays but not pure exposure.

**Economics:** Pilz and Sick are private — the publicly investable expression of safety is via ABB, Schneider (Pelco), Rockwell, Siemens, and Omron. Functional safety silicon (Infineon, NXP) is a beneficiary.

### H. Robotics OEMs and integrators
- **Industrial:** Fanuc (6954.T / FANUY), ABB, Yaskawa (6506.T / YASKY), KUKA (Midea-owned, delisted), Kawasaki (7012.T), DENSO Robotics (captive), Staubli (private), Comau (Stellantis/now sold).
- **Humanoid:** Figure (private), 1X (private), Apptronik (private), Agility (private, Amazon-backed), Sanctuary (private), Unitree (private/China), Boston Dynamics (Hyundai), Tesla Optimus (TSLA).
- **Warehouse / AMR:** Symbotic (SYM), AutoStore (AUTO.OL), Kion (KGX.DE) / Dematic, Daifuku (6383.T), Honeywell Intelligrated, KUKA Swisslog, GreyOrange (private), Locus (private), Geek+ (private), Exotec (private).
- **Cobots:** Universal Robots (Teradyne), ABB YuMi/GoFa, Doosan Robotics (454910.KS), Techman (Quanta-owned), Fanuc CRX, Yaskawa HC, Franka (private).
- **Drones / defense:** AeroVironment (AVAV), Kratos (KTOS), Anduril (private), Shield AI (private), Skydio (private), Joby (JOBY) for eVTOL, Archer (ACHR).
- **Surgical:** Intuitive Surgical (ISRG), Stryker (SYK — Mako), Medtronic (MDT — Hugo), Johnson & Johnson (Ottava), Globus Medical (GMED), Asensus (ASXC, marginal).
- **Agricultural:** Deere (DE), AGCO (AGCO), Trimble (TRMB), Kubota (6326.T), CNH (CNH), Raven (acquired by CNH).

**Economics:** This is where the temptation to overpay is highest. The Japanese big-four (Fanuc, Yaskawa, Kawasaki, DENSO captive) and ABB are the only durable winners. Humanoid OEMs as a category are unlikely to deliver returns proportionate to today's hype.

### I. Physical AI software
- **Robot operating systems:** ROS / ROS 2 (Open Robotics, captured by Intrinsic/Alphabet then spun off), NVIDIA Isaac, Microsoft Robotics Suite (largely deprecated), industrial proprietary stacks.
- **Simulation:** NVIDIA Isaac Sim/Omniverse, Dassault DELMIA/SIMULIA, ANSYS, MathWorks (private), Coppelia, Gazebo.
- **Digital twins:** Siemens Xcelerator, Dassault 3DEXPERIENCE, PTC ThingWorx, Bentley, Hexagon (HXGBY).
- **Fleet management:** Largely captive or private (Locus, Geek+, 6 River, Symbotic SymBots Manager, Amazon proprietary).
- **Autonomy / task planning:** Bright Machines (private), Path Robotics (private), Vicarious (acquired by Alphabet), Anduril Lattice, Palantir Foundry (PLTR — defense + industrial).
- **Teleoperation:** Saronic (private), Sarcos (effectively gone), Boston Dynamics, Apptronik's tele-rigs; no clean public pure-play.

**Economics:** NVIDIA captures the dominant share of the *commercial* simulation and robot-training software profit pool today. Siemens, Dassault, ANSYS (now Synopsys) capture the digital-twin / CAE pool. PTC captures the mid-tier. PLTR is the closest thing to a Physical-AI-defense software pure-play.

---

## 3. Adoption Analysis — Category by Category

### C-1. Adoption Curve Summary Table

| Category | Current adoption | Primary problem | What unlocks next 5 yrs | What unlocks next 10 yrs | First public beneficiaries | Probably overhyped |
|---|---|---|---|---|---|---|
| **Humanoids** | Pilot / pre-commercial (~2K–5K units cumulative shipped globally end-2025, mostly Unitree/Agility/Figure pilots) | General-purpose form factor cannot yet justify $30–80K BOM vs. $15/hr labor | Foundation-model dexterity, battery density, BOM cost down to ~$25K | Mass deployment in warehouse and 3PL; $10–15K BOM | NVDA, FANUY, YASKY, ABB, ADI, MPWR, HRL (Harmonic Drive private/JP), Nidec (JP) | Most humanoid private OEMs at >$10B valuation; pure SPAC plays |
| **Warehouse robotics** | Significant: Amazon ~1M+ robots; broader industry ~5–10% of warehouses meaningfully automated | Labor scarcity, throughput per sq ft | Symbotic/AutoStore-class systems scale; AMRs ubiquitous in mid-size DCs | Goods-to-person becomes default; lights-out micro-fulfillment | SYM, ZBRA, HON, KION (KGX.DE), AUTO.OL | Generic "AI warehouse robot" SPACs; standalone AMR startups |
| **Industrial cobots** | Mid-curve: ~80K units/year globally, ~10–12% of total robot installations | Programming complexity, payload limits, cycle time | Easier programming via VLA; better force/torque; payloads to 30 kg | Cobots become majority of new installs | TER (UR/MiR), FANUY (CRX), ABB (GoFa/YuMi), YASKY (HC), Doosan Robotics, Techman | Pure cobot SPACs and unprofitable late-stage entrants |
| **Autonomous mobile robots (AMRs)** | Real and accelerating in logistics; nascent in hospitality and last-mile | Indoor SLAM works; outdoor mixed environments hard | Multi-vendor fleet management; standardized safety | Mass last-mile delivery in select geos | TER (MiR), ZBRA, SYM, SERV (last-mile), HON, KION/Dematic | Sidewalk-robot SPACs; teleoperation-as-a-service plays |
| **Factory automation** | Mature in autos, semis, batteries; under-penetrated in SMB | Capital expense, integrator scarcity, mix complexity | EV/battery wave, reshoring; cobot integration | India + ASEAN automation wave | SIEGY, ABBNY, ROK, FANUY, YASKY, OMRNY, MIELY, SU.PA | Generic "smart factory" themed ETFs over individual incumbents |
| **Logistics automation** | Moderate; concentrated at Amazon, Walmart, large 3PLs | Throughput, peak surge, labor scarcity | Symbotic-class deployments scale; AS/RS retrofits | Lights-out DCs become default for top 50 retailers | SYM, ZBRA, HON, KION, DSV (operator), MAERSK-B (operator) | Subscale AMR/AS-RS vendors |
| **Defense drones & autonomy** | Live combat use (Ukraine), early procurement at scale | Procurement cycles, EW resistance, autonomy regulation | Loitering munitions standardization; small-drone swarms | Autonomous tactical fleets; replicator-class programs | AVAV, KTOS, LMT, RTX, GD, PLTR (software), Anduril (private) | Pure-play "defense AI" SPACs without programs of record |
| **Surgical robots** | Mature (>2M da Vinci procedures/yr); broadening to bone, soft-tissue, endoluminal | Capital cost, surgeon training, reimbursement | Da Vinci 5 + Ion penetration; soft-tissue from MDT/SYK/JNJ | Modular smaller systems; outpatient penetration | ISRG, SYK (Mako), MDT (Hugo), JNJ (Ottava), GMED | Asensus and other subscale challengers |
| **Agricultural robotics** | Tractor autonomy real (Deere See & Spray, AutoTrac); harvest robotics nascent | Cost/acre, weather, labor disruption | Vision-spray and autonomous tractors in row crops | Specialty-crop harvest; autonomous orchards | DE, AGCO, TRMB, KUBOTA (6326.T), CNH | Pure-play "ag-tech" specialty harvesters at venture stage |
| **Inspection robots** | Niche but real (utility, oil & gas, mining) | Battery life, certification, integration with asset systems | Drone/dog hybrid inspections; Spot-class deployments | Fully autonomous infrastructure inspection | BA, RTX (some), AVAV, FLIR (Teledyne TDY) | Inspection-as-a-service startups; Spot copycat OEMs |

### C-2. Per-category narrative analysis

#### Humanoids
**Problem solved:** A general-purpose, bipedal robot that can operate in human-shaped environments (warehouses, factories, eventually homes) without infrastructure change. The ROI case is *labor displacement* — currently theoretical at meaningful scale.

**Where we actually are (mid-2026):** Cumulative humanoid units shipped globally are still <10K. Most "deployments" are paid pilots at single customers (BMW with Figure, Mercedes with Apptronik, GXO with Agility, Amazon with Agility/Digit). Unit BOM costs are widely cited at $30–80K for premium designs and $10–25K for Unitree-class. **No humanoid manufacturer has demonstrated sustained per-hour productivity exceeding $15/hr labor on the same task at acceptable defect rates.** This is the most important fact in the entire Physical AI debate, and it is routinely glossed over.

**Five-year unlock:** Foundation-model dexterity (the π-class and GR00T-class VLA models). Battery density 10–20% improvement. Component cost declines as humanoid-specific supply chains (esp. harmonic reducers, frameless torque motors) scale. Plausible cumulative shipments by 2030: 100K–500K units.

**Ten-year unlock:** True $10–15K BOM costs (analogous to scooter-economics), enabling labor-cost parity in 24/7 warehouse and 3PL environments. Plausible cumulative shipments by 2035: 5M–20M units (extremely wide range; the bull case is real but not central).

**First public beneficiaries:** NVIDIA (Jetson Thor + Isaac), Fanuc/Yaskawa (servo motors + decades of robotics IP), ABB (factory integration), Analog Devices (motor control + IMUs), Monolithic Power (drive electronics), Harmonic Drive Systems (reducers — though ADR liquidity is poor), Nidec (motors). **Tesla is an optionality play, not a fundamentals play, for Optimus.**

**Probably overhyped:** Most humanoid OEM private valuations. The category will likely look like the EV-startup category in 2020–2024 — a few winners, many failures. Public investors should bet on the **component layer** until OEM economics are demonstrated.

#### Warehouse robotics
**Problem solved:** Throughput per square foot, labor scarcity at $20–25/hr fully-loaded, peak surge handling. The category includes AS/RS (Symbotic, AutoStore, Dematic, Daifuku, Murata), AMRs (Locus, MiR/Teradyne, 6 River, Geek+), and end-of-line robotics (Berkshire Grey, RightHand).

**Where we are:** ~5–10% of US/EU warehouses are *meaningfully* automated. Amazon Robotics is in a class of its own (1M+ drives, captive). Symbotic has demonstrated economics at Walmart and Target.

**Five-year unlock:** AS/RS retrofits in mid-size DCs become standard; multi-vendor fleet management matures.

**Ten-year unlock:** Lights-out micro-fulfillment in dense urban markets.

**First public beneficiaries:** Symbotic (SYM) — but with extreme customer concentration to Walmart. Zebra (ZBRA), Honeywell (Intelligrated), Kion (KGX.DE)/Dematic, AutoStore (AUTO.OL). **AutoStore is the cleanest non-US warehouse-robotics pure-play.**

**Probably overhyped:** Symbotic at peak multiples (the Walmart relationship is also the ceiling); pure-play AMR vendors with subscale fleets.

#### Industrial cobots
**Problem solved:** Robots that work alongside humans without fencing — used for assembly, machine tending, pick-and-place, palletizing. The fastest-growing slice of industrial robotics.

**Where we are:** ~80K cobot units shipped globally in 2024 (approx., per IFR), ~12% of total industrial robot installations. Universal Robots (Teradyne) is share leader, Fanuc CRX gaining quickly.

**Five-year unlock:** VLA-driven programming-by-demonstration; higher payloads; faster cycle times.

**First public beneficiaries:** Teradyne (UR), Fanuc, ABB, Yaskawa, Doosan Robotics.

#### Defense drones & autonomy
**Problem solved:** Persistent ISR, loitering munitions, counter-UAS, autonomous logistics in contested environments. Ukraine has provided 3+ years of combat-validated data points.

**Where we are:** US Replicator program in execution. Hundreds of thousands of small drones consumed in Ukraine annually. Public companies: AeroVironment (Switchblade, JUMP 20, Puma), Kratos (Valkyrie XQ-58, target drones), Lockheed/Raytheon/GD/Northrop on larger platforms, Palantir on software backbone, BAE on EW.

**Five-year unlock:** Programs of record for autonomous tactical fleets; software-defined drones.

**Ten-year unlock:** Replicator-class autonomous formations as standard force structure.

**First public beneficiaries:** AVAV, KTOS, PLTR, LMT, RTX, GD. **AVAV is the most direct small-drone pure-play.**

**Probably overhyped:** Defense-AI SPACs without programs of record.

#### Surgical robotics
**Problem solved:** Minimally invasive surgery with better dexterity than laparoscopic tools; orthopedic precision (Mako).

**Where we are:** ISRG da Vinci has >9,500 systems installed globally; 2M+ procedures/year. Stryker Mako dominant in knee/hip. MDT Hugo, JNJ Ottava emerging.

**Five-year unlock:** Da Vinci 5 conversion cycle; soft-tissue penetration by MDT/JNJ.

**First public beneficiaries:** ISRG (dominant), SYK, MDT, JNJ. **ISRG is the single highest-quality Physical AI franchise in public markets.**

---

## 4. Bottleneck Analysis — Where the Economics Accrue

The structural question for every Physical AI layer is the same: **what is the scarce, hard-to-replicate, certified, sticky asset?**

| Layer | True bottleneck | Who captures economics | Who gets commoditized | What is scarce | What becomes cheap | Mostly marketing |
|---|---|---|---|---|---|---|
| **Robot brain / training** | Compute + simulation tooling + data | NVIDIA (Jetson + Isaac + Cosmos + Omniverse); cloud providers for training compute | Open-source ROS forks; small VLA labs without compute access | Long-tail dexterous-manipulation data; compute for VLA training | Open VLA model weights | "AI-native robotics company" naming |
| **Embedded compute** | Power/perf envelope at ~50–200W; auto-grade qualification | NVIDIA (Jetson Thor); QCOM (RB platform); NXP, STM, Renesas, Infineon for MCUs | Generic ARM SoC vendors; smaller robotics-SoC startups | ISO 26262 / IEC 61508 certification | Generic edge inference TOPS | "Robotics SoC startup" without OEM design wins |
| **Sensing** | Sensor performance × cost × certification | Cognex (vision); ADI, STM, Bosch (IMU); NXP, Infineon, TI (radar) | Lidar pure-plays; commodity camera modules | Calibrated radar at scale; safety-rated vision | Lidar units; basic 2D cameras | "AI-camera" startups |
| **Motion / actuation** | Harmonic reducers; frameless torque motors; servo drives | Harmonic Drive Systems, Nabtesco (reducers); Fanuc, Yaskawa, Nidec, Maxon (motors); ABB (drives); ADI, ALGM, MPWR (silicon) | Generic servo OEMs without motion-control SW | Strain-wave gears; high-pole-count frameless torque motors | Generic stepper motors and basic drives | Generic actuator startups |
| **Industrial automation** | Installed base, fieldbus, integrator network | Siemens (Profinet/Simatic); Rockwell (EtherNet/IP/Logix); ABB; Schneider; Mitsubishi; Omron | Greenfield PLC startups | 30-year installed base relationships | Generic remote I/O | "Industrial cloud" branding without protocol depth |
| **Safety / validation** | Certifications (TÜV, UL, ISO 26262, IEC 61508, ISO 10218) | Pilz (private), Sick, ABB, Rockwell, Keyence | Uncertified safety vendors | Certified parts and integrators | Generic e-stop hardware | "Safety AI" without TÜV cert |
| **Test & measurement** | Validation tooling for autonomous systems and silicon | KEYS, TER (and to a lesser extent ANSS/Synopsys, CDNS) | Generic O-scope vendors | EV/auto/robotics test chambers | Bench instruments | "Autonomy test platform" SaaS without industrial customers |
| **Robotics OEMs (industrial)** | Reliability + sales/service network + 30-year track record | Fanuc, ABB, Yaskawa, Kawasaki | Mid-tier and Chinese OEMs (Estun, Inovance) climbing | Premium reliability; integrator relationships | Asian mid-tier 6-axis robots | Western humanoid OEMs in 2025 vintage |
| **Robotics OEMs (humanoid)** | Reaching $10–15K BOM with reliable operation | TBD — likely 2–5 winners globally | Most | Reliable hand/finger dexterity | Mid-tier humanoid form factors | Most current valuations |
| **Physical AI software** | Simulation fidelity + integration | NVIDIA (Isaac/Omniverse); Siemens/Dassault/ANSYS (digital twin); PLTR (defense) | Generic ROS distros and small fleet-mgmt vendors | High-fidelity contact-rich simulation | Generic ROS deployments | "AI robot platform" SaaS without industrial deployments |
| **Drones / defense autonomy** | Programs of record; classified-environment integration | LMT, RTX, GD, NOC, AVAV, KTOS, PLTR | Small defense-tech SPACs | Defense procurement contracts | Commercial drone hardware | Pre-program defense-AI startups |
| **Surgical robotics** | Installed base, training network, consumables | ISRG (dominant); SYK (ortho); MDT, JNJ (emerging) | Subscale challengers (ASXC) | Installed da Vinci base; surgeon training | Generic articulated arms | "AI surgery" without FDA approvals |
| **Warehouse / logistics** | Customer relationships + system integration + WMS | SYM (concentrated to WMT), KION/Dematic, AUTO.OL, Daifuku, HON, ZBRA | AMR startups without anchor customers | Anchor enterprise contracts | Generic AMRs | Generic warehouse-AI startups |
| **Power management** | Mixed-signal IP + reference designs + automotive qualification | MPWR, ADI, TXN, Infineon | Generic LDO/regulator vendors | Automotive-grade motor power IC | Commodity DC-DC | "AI power" branding |

**The pattern is consistent:** Economics accrue to (1) **certified, installed-base, hard-to-replicate component layers** — sensors, motion control, embedded silicon, automation incumbents — and (2) **one or two true platform layers** — NVIDIA Isaac on the AI side, and the surgical-robotics monopoly on the application side. Robot OEMs at the *new* end (humanoids) are unlikely to capture proportionate economics.

---

## 5. Public Equity Universe — Categorized

Tickers below are organized by primary subsector. (Ticker, name, primary listing, approx. mkt cap, where it lives in the stack.) All figures approximate, late-2024 to FY2025 reporting.

### 5.1 Robot brain / foundation models / simulation
- **NVDA** — NVIDIA — US — ~$3T+ — Jetson, Isaac, GR00T, Cosmos, Omniverse. The dominant exposure.
- **DASTY / DSY.PA** — Dassault Systèmes — France — ~$40B — DELMIA/SIMULIA digital twin.
- **PTC** — PTC Inc. — US — ~$20B — ThingWorx/Onshape/Vuforia.
- **HXGBY / HEXA-B.ST** — Hexagon AB — Sweden — ~$25B — Sensors, software, autonomous mining.
- **SNPS** — Synopsys — US — ~$80B — ANSYS-integrated simulation post-acquisition.

### 5.2 Embedded compute / robotics SoCs
- **NVDA** — Jetson Orin/Thor.
- **QCOM** — Qualcomm — US — ~$180B — Robotics RB platform; auto Snapdragon Ride.
- **AMBA** — Ambarella — US — ~$2B — CVflow vision SoCs for cameras/drones.
- **NXPI** — NXP — Netherlands — ~$55B — Auto + industrial MCUs, S32 platform.
- **STM** — STMicroelectronics — France/Italy — ~$25B — MCUs, drivers, IMUs.
- **MCHP** — Microchip — US — ~$30B — Industrial MCUs.
- **TXN** — Texas Instruments — US — ~$170B — Analog, MCUs, TDA4 robotics platform.
- **RNECY / 6723.T** — Renesas — Japan — ~$25B — Auto/industrial MCUs.
- **IFNNY / IFX.DE** — Infineon — Germany — ~$45B — Power, sensors, MCUs, safety.

### 5.3 Sensing & perception
- **CGNX** — Cognex — US — ~$6B — Pure-play machine vision.
- **KYCCF / 6861.T** — Keyence — Japan — ~$140B — Best-in-class machine vision/sensing; premium multiple.
- **ADI** — Analog Devices — US — ~$110B — MEMS IMU, sensing analog.
- **TDK / 6762.T** — TDK Corp — Japan — ~$25B — InvenSense IMUs.
- **HSAI** — Hesai — China/US-listed — ~$1B — Lidar.
- **OUST** — Ouster — US — ~$700M — Lidar.
- **INVZ** — Innoviz — Israel — small cap — Lidar.
- **LAZR** — Luminar — US — small cap — Lidar (struggling).
- **AEVA** — Aeva — US — small cap — FMCW lidar.
- **TDY** — Teledyne — US — ~$22B — DALSA, FLIR thermal, Imaging.

### 5.4 Motion & actuation
- **ALGM** — Allegro MicroSystems — US — ~$5B — Magnetic sensors, motor driver ICs.
- **NJDCY / 6594.T** — Nidec — Japan — ~$30B — Motors at scale; humanoid actuator exposure.
- **MAXN.SW** — Maxon (private; Maxon Group is private) — Switzerland — Premium brushless motors. *Not publicly listed in clean form.*
- **6324.T** — Harmonic Drive Systems — Japan — small/mid cap — Strain-wave gear monopoly. *No clean ADR.*
- **6268.T** — Nabtesco — Japan — ~$3B — RV reducers.
- **MOG.A / MOG.B** — Moog Inc — US — ~$6B — Precision motion for aerospace/defense.
- **PH** — Parker Hannifin — US — ~$80B — Motion and control conglomerate (hydraulics, electromechanical).

### 5.5 Industrial automation incumbents
- **SIEGY / SIE.DE** — Siemens — Germany — ~$170B — Simatic, SINUMERIK, Xcelerator.
- **ABBNY / ABBN.SW** — ABB — Switzerland — ~$110B — Robotics, drives, motion, process automation.
- **ROK** — Rockwell Automation — US — ~$30B — Logix, PLCs, FactoryTalk.
- **SBGSY / SU.PA** — Schneider Electric — France — ~$130B — AVEVA software, EcoStruxure, motion.
- **OMRNY / 6645.T** — Omron — Japan — ~$15B — Industrial automation, sensing, safety.
- **MIELY / 6503.T** — Mitsubishi Electric — Japan — ~$45B — FA, drives, MELSEC PLCs.
- **EMR** — Emerson — US — ~$70B — Process automation (post-Test&Measurement spin to Veralto/AMETEK).
- **FTV** — Fortive — US — ~$25B — T&M, sensors (Tektronix, Fluke).
- **DOV** — Dover — US — ~$25B — Industrial conglomerate.
- **HON** — Honeywell — US — ~$140B — Intelligrated, process, Forge software.

### 5.6 Safety / validation / cybersecurity
- (Pilz, Sick, TÜV, UL all private.) Publicly: **ABB, ROK, Siemens, OMRNY, Schneider** (safety divisions); **IFNNY, NXPI, STM, RNECY** (functional safety silicon); **PANW, CRWD** (OT cyber partnerships, not pure plays).

### 5.7 Test & measurement
- **KEYS** — Keysight — US — ~$30B — Autonomous systems test, RF, EV, semis.
- **TER** — Teradyne — US — ~$20B — Semi test + Universal Robots (cobots) + MiR (AMRs).
- **CGNX** — Cognex — also a metrology play.
- **FTV** — Fortive — broad T&M.
- **ANSS** — ANSYS — now part of SNPS (Synopsys).
- **NATL / NATI** — formerly National Instruments, now Emerson-owned (delisted).

### 5.8 Robotics OEMs (industrial / cobot / AMR / warehouse / surgical / drones)
- **FANUY / 6954.T** — Fanuc — Japan — ~$40B — Industrial robots, CNC, factory automation.
- **YASKY / 6506.T** — Yaskawa — Japan — ~$10B — Servomotors, drives, robotics.
- **ABBNY** — ABB — also robot OEM.
- **TER** — Teradyne — UR (cobots) + MiR (AMRs) inside ATE shell.
- **SYM** — Symbotic — US — ~$15B (volatile) — Warehouse automation, heavy Walmart concentration.
- **AUTO.OL** — AutoStore — Norway — ~$3B — Cube-storage AS/RS.
- **KGX.DE** — Kion Group — Germany — ~$5B — Forklifts + Dematic (warehouse).
- **6383.T** — Daifuku — Japan — ~$10B — Material handling.
- **ZBRA** — Zebra Technologies — US — ~$15B — Scanning, RFID, mobile computing.
- **HON** — Honeywell — also Intelligrated.
- **ISRG** — Intuitive Surgical — US — ~$160B — Surgical robotics monopoly.
- **SYK** — Stryker — US — ~$140B — Mako orthopedic.
- **MDT** — Medtronic — US — ~$110B — Hugo + Mazor + adjacencies.
- **GMED** — Globus Medical — US — ~$10B — Spine robotics.
- **AVAV** — AeroVironment — US — ~$5B — Switchblade, JUMP 20, Puma.
- **KTOS** — Kratos — US — ~$3B — XQ-58 Valkyrie, target drones.
- **454910.KS** — Doosan Robotics — Korea — cobots.

### 5.9 Power management
- **MPWR** — Monolithic Power — US — ~$25B — Mixed-signal power management.
- **ADI** — Analog Devices — also motor + power.
- **TXN** — Texas Instruments — power, analog, motor.
- **IFNNY** — Infineon — power, SiC.
- **ON** — onsemi — US — ~$30B — SiC, image sensors, power.
- **WOLF** — Wolfspeed — US — small cap — SiC pure-play but balance-sheet stressed.
- **VSH** — Vishay — US — ~$3B — Discretes.
- **STM** — STMicro — also SiC.

### 5.10 Agricultural and precision
- **DE** — Deere — US — ~$130B — Autonomous tractors, See & Spray.
- **AGCO** — AGCO — US — ~$7B — Fendt, PTx Trimble.
- **TRMB** — Trimble — US — ~$15B — Precision GNSS, machine control.
- **CNH** — CNH Industrial — US — ~$13B — Case IH, New Holland, autonomous AG.
- **6326.T / KUBTY** — Kubota — Japan — ~$20B — Compact agricultural autonomy.

### 5.11 Defense autonomy adjacencies (large primes)
- **LMT** — Lockheed Martin — ~$110B — Skunk Works autonomy programs.
- **RTX** — RTX Corp — ~$160B — Multiple programs, missiles.
- **GD** — General Dynamics — ~$80B — Robotics, autonomous ships.
- **NOC** — Northrop Grumman — ~$70B — UAVs, autonomy.
- **PLTR** — Palantir — ~$60–120B (volatile) — Defense + industrial autonomy software (Maven, Lattice partnerships).
- **AXON** — Axon — US — ~$30B — Tasers, drones (Sky-Hero), body cams.

---

## 6. Private-Market Context — Why Public Access is Imperfect

The following private companies represent the largest concentrations of Physical AI venture capital in the 2023–2026 vintages. For each, this section maps the public-market enablers and competitive linkages.

| Private company | What they do | Closest public proxy / supplier | Public competitor / acquirer candidate |
|---|---|---|---|
| **Figure AI** | Humanoid OEM; BMW pilot; OpenAI partnership (lapsed); ~$2.6B raised | NVDA (compute), TSLA-adjacent | Toyota, Honda, Hyundai (BD parent), Microsoft (investor) |
| **Physical Intelligence (π)** | Foundation models for robots (π₀, π-0.5) | NVDA (compute) | Could be acquired by Google/Microsoft/Amazon |
| **Agility Robotics** | Digit humanoid; GXO/Amazon pilots | TER (related space), NVDA | Amazon (investor; ultimate acquirer likely) |
| **Boston Dynamics** | Spot, Atlas (now electric), Stretch | NVDA, Hyundai-owned (005380.KS) | Hyundai — listed in Korea |
| **Unitree** | Low-cost humanoids and quadrupeds; China | None clean | Chinese listings; potential US export controls |
| **Skild AI** | Cross-embodiment foundation models | NVDA | Likely M&A target by an OEM or hyperscaler |
| **Covariant** | Industrial manipulation models | Was — Amazon hired key talent in mid-2024 ("acqui-hire") | AMZN absorbed |
| **1X** | Humanoid (Neo) for consumer | NVDA, OpenAI-backed | Could M&A to a consumer brand |
| **Sanctuary AI** | Phoenix humanoid | NVDA | Magna International (MGA — partner) |
| **Tesla Optimus** | (Public via TSLA) | TSLA — but Optimus is optionality | N/A |
| **Apptronik** | Apollo humanoid; Mercedes pilot; Google DeepMind partnership | NVDA, GOOG (partner) | Likely M&A target |
| **Anduril** | Defense autonomy (Lattice software, Roadrunner, Ghost, Bolt, Dive-LD) | PLTR (software adjacency), LMT/RTX/GD (competitors) | Potential IPO or strategic acquisition |
| **Shield AI** | Autonomous flight stack (Hivemind), V-BAT | AVAV (small drones), KTOS | M&A or IPO |
| **Skydio** | Autonomous drones | AVAV, AXON (Sky-Hero), defense primes | M&A by defense prime |
| **Saronic** | Autonomous surface vessels | LMT, GD (Bath Iron Works) | M&A target |

**Why public-market access is imperfect:** The most-cited Physical AI companies are private and likely to remain so until 2027–2029. Public investors must therefore express the thesis through:
1. **Component suppliers** to the private players (NVDA, ADI, MPWR, NXPI, the Japanese motion-control universe).
2. **Likely acquirers** (large autos, defense primes, automation incumbents, hyperscalers).
3. **Adjacent fully-public franchises** (ISRG in surgical, AVAV/KTOS in defense, Symbotic in warehouse).

---

## 7. Subsector Investment Framework

One table per subsector, per mandate.

### 7.1 Robot brain / simulation
| Field | Detail |
|---|---|
| Bottleneck | Compute access + simulation fidelity + training data |
| Best public expression | **NVDA** — Jetson + Isaac + Cosmos + Omniverse stack |
| Second-best | **DASTY** (Dassault Systèmes) — digital-twin simulation |
| Trap stock | Pure-play "AI robot platform" SPACs; smaller simulation startups |
| Underappreciated | **PTC** — modest valuation, real digital-twin / AR-for-industrial business |
| Private to watch | Physical Intelligence, Skild AI |
| 5-year outlook | NVDA dominance compounds; digital-twin demand grows steadily |
| 10-year outlook | Plausible margin compression as open-source VLA matures, but NVDA likely still owns the commercial stack |
| Rating | **OVERWEIGHT** (via NVDA, modest position) |

### 7.2 Embedded compute / robotics SoCs
| Field | Detail |
|---|---|
| Bottleneck | Power-efficient inference at automotive/industrial qualification grade |
| Best public expression | **NVDA Jetson** (within NVDA), **NXPI** for MCUs |
| Second-best | **STM**, **TXN** |
| Trap stock | **AMBA** — small, lumpy, but a genuine vision-SoC franchise; not a trap so much as binary |
| Underappreciated | **NXPI** — broad humanoid/cobot embedded exposure at industrial-grade |
| Private to watch | Hailo, Tenstorrent (for inference) |
| 5-year outlook | Volume growth in robot/auto/industrial sockets |
| 10-year outlook | Consolidation among MCU vendors continues |
| Rating | **OVERWEIGHT** (NXPI, ADI, NVDA via existing positions) |

### 7.3 Sensing / perception
| Field | Detail |
|---|---|
| Bottleneck | Cost × performance × certification at scale |
| Best public expression | **CGNX** — pure-play machine vision |
| Second-best | **KYCCF (Keyence)** if you can stomach the multiple; **ADI** for MEMS IMUs |
| Trap stock | **LAZR**, **OUST**, **INVZ**, **AEVA** — lidar pure-plays still cash-burning; differentiation eroding |
| Underappreciated | **TDY** (Teledyne) — FLIR + DALSA, undervalued imaging franchise |
| Private to watch | Bosch Sensortec, Sick |
| 5-year outlook | Vision/IMU steady; lidar continues to commoditize |
| 10-year outlook | Tactile / force-torque sensing becomes a bigger profit pool — but mostly private today |
| Rating | **OVERWEIGHT** Cognex + ADI; **AVOID** lidar pure-plays except as satellite |

### 7.4 Motion / actuation
| Field | Detail |
|---|---|
| Bottleneck | High-pole-count frameless torque motors + strain-wave reducers + servo drives |
| Best public expression | **FANUY** (servos, robots, motion-control software stack) |
| Second-best | **YASKY** + **ABBNY** + **ALGM** (drive silicon) |
| Trap stock | Generic motor OEMs without motion-control SW |
| Underappreciated | **ALGM** — magnetic sensing + motor driver ICs sit in every actuator |
| Private to watch | Harmonic Drive Systems (Japan-listed; no clean ADR), Maxon |
| 5-year outlook | Humanoid demand on top of existing factory demand — modest tailwind |
| 10-year outlook | This is where the *largest* dollar-content uplift hides if humanoids scale |
| Rating | **OVERWEIGHT** — Fanuc/Yaskawa/ABB/Allegro |

### 7.5 Industrial automation incumbents
| Field | Detail |
|---|---|
| Bottleneck | Installed base + fieldbus + integrator network |
| Best public expression | **SIEGY** + **ABBNY** |
| Second-best | **ROK**, **Schneider** (SBGSY/SU.PA) |
| Trap stock | Pure "smart factory ETF" exposure over individual names |
| Underappreciated | **OMRNY** (Omron) — Japan-listed, undervalued |
| Private to watch | Beckhoff, Bosch Rexroth, Pilz |
| 5-year outlook | EV/battery wave + reshoring drives capex |
| 10-year outlook | India + ASEAN automation wave; PLC -> edge convergence; software margin expansion |
| Rating | **OVERWEIGHT** — backbone of the portfolio |

### 7.6 Safety / validation
| Field | Detail |
|---|---|
| Bottleneck | Certification (TÜV, ISO 13849, ISO 10218, IEC 61508, ISO 26262) |
| Best public expression | **OMRNY** (broadest safety portfolio in public Japanese), **ABB** (Jokab) |
| Second-best | **ROK** (Guardmaster) |
| Trap stock | "Safety AI" without TÜV certifications |
| Underappreciated | Functional-safety silicon at **IFNNY, NXPI** |
| Private to watch | Pilz, Sick, Schmersal |
| 5-year outlook | Humanoid certification frameworks are nascent — material regulatory tailwind ahead |
| 10-year outlook | Robot-cert becomes its own profit pool |
| Rating | **MARKET WEIGHT** — capture via incumbents |

### 7.7 Test & measurement
| Field | Detail |
|---|---|
| Bottleneck | EV/auto/robotics validation tooling at industrial scale |
| Best public expression | **KEYS** — Keysight |
| Second-best | **TER** (when ATE cycle cooperates) |
| Trap stock | "Autonomy simulation SaaS" without industrial customers |
| Underappreciated | **FTV** — Fluke/Tektronix franchise |
| Private to watch | dSPACE (private), Applied Intuition (private) |
| 5-year outlook | Robotics validation demand grows; EV cycle volatile |
| 10-year outlook | Autonomous-system certification testing becomes a structurally larger market |
| Rating | **OVERWEIGHT** — Keysight is a mansion candidate |

### 7.8 Robotics OEMs
| Field | Detail |
|---|---|
| Bottleneck | Reliability + sales/service + multi-decade IP |
| Best public expression | **FANUY** |
| Second-best | **ABBNY**, **YASKY** |
| Trap stock | Humanoid OEM SPACs and any "robot OEM" with no anchor customer |
| Underappreciated | **TER** — Universal Robots is durable cobot leader inside an ATE shell |
| Private to watch | Boston Dynamics (Hyundai), Apptronik, Figure |
| 5-year outlook | Industrial robotics steady-growth; humanoids non-material to revenue |
| 10-year outlook | Possible humanoid revenue lift for incumbents that bring component IP |
| Rating | **OVERWEIGHT** — Fanuc and Teradyne |

### 7.9 Physical AI software
| Field | Detail |
|---|---|
| Bottleneck | Simulation fidelity + multi-vendor integration |
| Best public expression | **NVDA** Isaac/Omniverse (already covered above) |
| Second-best | **SIEGY** Xcelerator |
| Trap stock | Standalone "robot software" SaaS without OEM endorsements |
| Underappreciated | **PTC** — meaningful AR/digital-twin franchise at reasonable multiple |
| Private to watch | Intrinsic (Alphabet), Bright Machines |
| 5-year outlook | NVDA owns the platform; digital twins steady growth |
| 10-year outlook | Possible disintermediation by open-source — but commercial enterprises pay for support |
| Rating | **MARKET WEIGHT** — captured via NVDA + Siemens |

### 7.10 Drones / defense autonomy
| Field | Detail |
|---|---|
| Bottleneck | Programs of record + classified integration |
| Best public expression | **AVAV** + **KTOS** (pure-plays); **LMT/RTX/GD** for large platform exposure |
| Second-best | **PLTR** for software backbone |
| Trap stock | Defense-AI SPACs without programs |
| Underappreciated | **MOG.A** — Moog's precision actuation goes into many autonomous platforms |
| Private to watch | Anduril, Shield AI, Saronic, Skydio |
| 5-year outlook | US Replicator program + allied procurement = strong |
| 10-year outlook | Autonomous formations as standard force structure |
| Rating | **OVERWEIGHT** — but via satellites (AVAV, KTOS), not mansion |

### 7.11 Surgical robotics
| Field | Detail |
|---|---|
| Bottleneck | Installed base + surgeon training + consumables stream |
| Best public expression | **ISRG** |
| Second-best | **SYK** (Mako), **MDT** (Hugo) |
| Trap stock | Asensus (ASXC) |
| Underappreciated | **GMED** — spine robotics (Excelsius), smaller but durable |
| Private to watch | Vicarious Surgical (declined), CMR Surgical (UK private) |
| 5-year outlook | Da Vinci 5 conversion cycle; Hugo/Ottava ramp |
| 10-year outlook | Soft-tissue penetration outside US; outpatient |
| Rating | **OVERWEIGHT** — ISRG is the mansion anchor |

### 7.12 Warehouse / logistics automation
| Field | Detail |
|---|---|
| Bottleneck | Customer relationships + WMS integration + reliability at peak |
| Best public expression | **SYM** with caveats; **AUTO.OL**, **KGX.DE** |
| Second-best | **ZBRA**, **HON** (Intelligrated), **6383.T** (Daifuku) |
| Trap stock | SYM if Walmart relationship rerates negatively |
| Underappreciated | **KGX.DE** (Kion) — Dematic franchise plus forklift base |
| Private to watch | Geek+, Locus, Exotec |
| 5-year outlook | Continued double-digit growth in DC automation |
| 10-year outlook | Lights-out micro-fulfillment in dense markets |
| Rating | **OVERWEIGHT** — via Symbotic (satellite) + Zebra (middle) |

### 7.13 Power management
| Field | Detail |
|---|---|
| Bottleneck | Mixed-signal IP + automotive qualification |
| Best public expression | **MPWR** |
| Second-best | **ADI**, **TXN**, **IFNNY** |
| Trap stock | **WOLF** — SiC pure-play with balance-sheet stress |
| Underappreciated | **ON** — image sensors + SiC + power |
| Private to watch | None of significant scale |
| 5-year outlook | Steady volume growth in industrial + EV + robotics |
| 10-year outlook | Humanoid power-density demand becomes a real driver |
| Rating | **OVERWEIGHT** — MPWR (middle), ADI (middle) |

---

## 8. Mansion Candidate Scoring

Each mansion candidate is scored 1–10 on ten dimensions. **Higher is better** on all except cyclicality risk, valuation risk, and geopolitical risk where the score reflects favorability (10 = low risk). All scores are subjective and reflect institutional judgment, not a formal model.

### 8.1 Selected mansion candidates (7)

| Candidate | Moat | Direct PAI relevance | Rev. visibility | Pricing power | Op. leverage | Cyclicality (10=low risk) | Valuation (10=cheap) | Geopolitical (10=low risk) | Balance sheet | 2030 relevance | **Total /100** |
|---|---|---|---|---|---|---|---|---|---|---|---|
| **ISRG** | 10 | 8 | 10 | 9 | 8 | 9 | 4 | 7 | 10 | 10 | **85** |
| **NVDA** | 10 | 7 | 9 | 10 | 10 | 5 | 3 | 4 | 10 | 9 | **77** |
| **ABBNY** (ABB) | 8 | 9 | 8 | 7 | 7 | 5 | 7 | 6 | 8 | 9 | **74** |
| **SIEGY** (Siemens) | 9 | 9 | 8 | 8 | 7 | 5 | 8 | 5 | 8 | 10 | **77** |
| **KEYS** | 8 | 7 | 7 | 7 | 6 | 5 | 7 | 6 | 8 | 8 | **69** |
| **CGNX** | 9 | 10 | 6 | 7 | 8 | 3 | 5 | 6 | 9 | 9 | **72** |
| **FANUY** | 9 | 10 | 6 | 7 | 9 | 3 | 7 | 5 | 10 | 9 | **75** |

### 8.2 Rejected mansion candidates (and rationale)

| Candidate | Reason for rejection from mansion sleeve |
|---|---|
| **TSLA** | Humanoid (Optimus) is optionality, not earnings. Auto core is not pure Physical AI. Valuation extreme. Better expressed via component suppliers. |
| **AMD** | Datacenter-GPU story; robotics SoC share immaterial relative to NVIDIA's Jetson/Isaac stack. |
| **INTC** | Not a durable Physical AI thesis; turnaround risk dominates. |
| **MBLY** | Auto-cycle exposure + ADAS competitive intensity; better as a satellite if at all. |
| **SYM (Symbotic)** | Severe customer concentration to Walmart; execution risk on backlog conversion. Belongs in satellite, not mansion. |
| **IRBT** | Structurally broken consumer robotics; not a Physical AI mansion. |
| **ROK** | Solid franchise but US-focused with limited Asia growth; mid-cap industrial cyclicality outweighs durable-monopoly status — middle sleeve instead. |
| **HON** | Diversified conglomerate; Physical AI exposure (Intelligrated) is <10% of revenue — middle sleeve. |
| **EMR** | Post-Test&Measurement spin focuses on process, not Physical AI proper. |
| **DOV** | Industrial conglomerate with too little direct Physical AI exposure to justify mansion. |
| **DE** | Real autonomy exposure but agricultural cycle dominates near-term — middle/satellite. |
| **YASKY** | High-quality but Fanuc and ABB occupy the limited mansion slots in OEM/automation sleeves; Yaskawa enters middle. |
| **HSAI / OUST / INVZ / LAZR / AEVA** | Lidar pure-plays — speculative, commoditizing — satellite only. |
| **AXON** | Solid franchise but predominantly police/Taser/body-cam; not a pure Physical AI mansion thesis. |
| **AVAV / KTOS** | Defense autonomy is real, but lumpy and program-cycle-driven — satellites. |
| **PLTR** | Defense + commercial software, real Physical AI adjacencies via Lattice partnerships and Maven — but valuation and revenue-concentration risk push out of mansion. |
| **ADI** | Excellent franchise and durable, but mansion slot best used on more direct-pure exposure (CGNX, FANUY) — middle sleeve at full size. |
| **MPWR** | Same logic as ADI — high quality, middle sleeve. |
| **NXPI** | Auto + industrial MCUs are central to Physical AI but auto-cycle risk and 20-25% China revenue exposure put it in middle sleeve. |
| **TER** | Excellent — UR/MiR + ATE — but exposure split between ATE (semis cycle) and robotics (real PAI). Middle. |
| **SBGSY (Schneider)** | Strong PAI franchise (AVEVA + EcoStruxure + motion) but ABB and Siemens already cover this sleeve; would breach the ≤2-per-subsector mansion rule. |
| **DASTY (Dassault)** / **PTC** | Strong digital-twin franchises but NVDA captures the lion's share of mansion-grade simulation exposure. |
| **TDY (Teledyne)** | Excellent imaging franchise but blended exposure (defense, scientific, marine) — mansion mismatch. |
| **TXN** | Quality is high but the analog/MCU cycle is in trough and recovery timing is uncertain — middle eligible, not mansion. |
| **GD / LMT / RTX / NOC** | Defense primes — Physical AI is a slice, not the thesis. |
| **KYCCF (Keyence)** | Arguably highest-quality sensing company globally, but ADR illiquidity and premium multiple keep it off the US-investor mansion list. |

---

## 9. The $500K Mansion Model Portfolio

Three variants, per the user's mandate.

### 9.1 Primary $500K Portfolio (the "Mansion Model")

| Ticker | Company | Sleeve | Subsector | $ Target | % of Portfolio | Role in Thesis | Risk |
|---|---|---|---|---|---|---|---|
| **ISRG** | Intuitive Surgical | Mansion | Surgical robotics | $50,000 | 10.0% | Highest-quality Physical AI franchise; recurring revenue; monopoly economics | Medium (valuation) |
| **NVDA** | NVIDIA | Mansion | Robot brain / sim | $50,000 | 10.0% | Robotics platform (Jetson/Isaac/GR00T/Cosmos/Omniverse); datacenter risk is the downside | Medium-High (valuation, cyclicality) |
| **ABBNY** | ABB | Mansion | Industrial automation incumbents | $42,000 | 8.4% | Robotics + drives + motion; integrator-network moat | Medium (industrial cycle) |
| **SIEGY** | Siemens | Mansion | Industrial automation incumbents | $42,000 | 8.4% | Simatic PLC + Xcelerator digital twin + motion control | Medium (industrial cycle, EU exposure) |
| **KEYS** | Keysight | Mansion | Test & measurement | $40,000 | 8.0% | Autonomous-system + EV + semis validation | Medium (semi capex cycle) |
| **CGNX** | Cognex | Mansion | Sensing / perception | $38,000 | 7.6% | Machine vision pure-play; structural moat | Medium-High (cyclical end markets) |
| **FANUY** | Fanuc | Mansion | Robotics OEMs | $38,000 | 7.6% | Industrial robot + CNC + servo motion; fortress balance sheet | Medium-High (factory cycle, China) |
| **ROK** | Rockwell Automation | Middle | Industrial automation | $18,000 | 3.6% | US-focused PLC dominance, software margin | Medium |
| **ADI** | Analog Devices | Middle | Sensing / motor | $18,000 | 3.6% | Best-in-class MEMS IMUs, mixed-signal motor control | Medium |
| **TER** | Teradyne | Middle | Robotics OEMs / T&M | $18,000 | 3.6% | UR (cobots) + MiR (AMRs) + ATE | Medium-High |
| **MPWR** | Monolithic Power | Middle | Power management | $15,000 | 3.0% | Motor + power management ICs | Medium |
| **AXON** | Axon Enterprise | Middle | Defense / public-safety autonomy | $15,000 | 3.0% | Tasers, drones (Sky-Hero), body cams; closest to "consumer defense autonomy" | Medium |
| **NXPI** | NXP Semiconductors | Middle | Embedded compute | $15,000 | 3.0% | Auto + industrial MCUs; S32 platform | Medium-High (auto cycle, China) |
| **ZBRA** | Zebra Technologies | Middle | Warehouse / logistics | $11,000 | 2.2% | Scanning, RFID, AMR adjacency | Medium-High |
| **HON** | Honeywell | Middle | Warehouse + industrial | $10,000 | 2.0% | Intelligrated, broad industrial exposure | Low-Medium |
| **SYM** | Symbotic | Satellite | Warehouse automation | $7,000 | 1.4% | Pure-play DC automation; high concentration risk to Walmart | High |
| **AVAV** | AeroVironment | Satellite | Defense autonomy | $6,000 | 1.2% | Switchblade/JUMP 20; small-drone pure-play | High |
| **ALGM** | Allegro MicroSystems | Satellite | Motion / sensing | $5,000 | 1.0% | Magnetic sensing + motor driver ICs; every actuator | Medium-High |
| **HSAI** | Hesai | Satellite | Sensing (lidar) | $5,000 | 1.0% | Best-positioned lidar pure-play; commoditization risk | High |
| **KTOS** | Kratos | Satellite | Defense autonomy | $4,000 | 0.8% | XQ-58 Valkyrie program; tactical drones | High |
| **SERV** | Serve Robotics | Satellite | Last-mile robotics | $3,000 | 0.6% | Speculative last-mile delivery thesis; small position | Very High |
| **CASH** | — | Cash | — | $50,000 | 10.0% | Dry powder; pullback optionality | — |
| **TOTAL** | | | | **$500,000** | **100.0%** | | |

**Constraint check (Primary):**
- Sleeve totals: Mansion $300K (60.0%), Middle $120K (24.0%), Satellite $30K (6.0%), Cash $50K (10.0%). All within bands.
- Mansion positions: 7 (within 6–8 band). ✓
- Mansion subsectors represented: Surgical, Robot brain/sim, Industrial automation (×2 — ABBNY & SIEGY), T&M, Sensing, Robotics OEMs = **6 distinct subsectors** (≥5). ✓
- ≤2 mansion positions per subsector: max is 2 (industrial automation). ✓
- Middle positions: 8 (within 6–10). ✓
- Satellite positions: 6 (within 5–8). ✓
- Cash: 9.6% (within 8–12%). ✓
- No duplicate tickers. ✓
- No company in multiple sleeves. ✓

### 9.2 Aggressive Variant (low cash, more humanoid/defense-autonomy upside)

| Ticker | Sleeve | Δ vs. Primary | $ Target | % |
|---|---|---|---|---|
| ISRG | Mansion | unchanged | $50,000 | 10.0% |
| NVDA | Mansion | +$5K (Cosmos/GR00T as humanoid optionality) | $55,000 | 11.0% |
| ABBNY | Mansion | unchanged | $42,000 | 8.4% |
| SIEGY | Mansion | unchanged | $42,000 | 8.4% |
| KEYS | Mansion | unchanged | $40,000 | 8.0% |
| CGNX | Mansion | unchanged | $38,000 | 7.6% |
| FANUY | Mansion | unchanged | $38,000 | 7.6% |
| ROK | Middle | -$4K | $14,000 | 2.8% |
| ADI | Middle | -$4K | $14,000 | 2.8% |
| TER | Middle | -$2K | $16,000 | 3.2% |
| MPWR | Middle | -$1K | $14,000 | 2.8% |
| AXON | Middle | -$1K | $14,000 | 2.8% |
| NXPI | Middle | -$3K | $12,000 | 2.4% |
| ZBRA | Middle | unchanged | $11,000 | 2.2% |
| HON | Middle | unchanged | $10,000 | 2.0% |
| SYM | Satellite | +$1K | $8,000 | 1.6% |
| AVAV | Satellite | +$2K | $8,000 | 1.6% |
| ALGM | Satellite | +$2K | $7,000 | 1.4% |
| HSAI | Satellite | unchanged | $5,000 | 1.0% |
| KTOS | Satellite | +$1K | $5,000 | 1.0% |
| SERV | Satellite | +$1K | $4,000 | 0.8% |
| **MOG.A** (new) | Satellite | new (defense actuation) | $7,000 | 1.4% |
| **TSLA** (new) | Satellite | new (Optimus optionality only) | $6,000 | 1.2% |
| CASH | Cash | -$10K | $40,000 | 8.0% |
| **TOTAL** | | | **$500,000** | **100.0%** |

Constraints: Mansion $305K (7 pos), Middle $105K (8 pos), Satellite $50K (8 pos at cap), Cash 8.0% at floor. ✓

### 9.3 Conservative Variant (high cash, automation + medical weighting)

| Ticker | Sleeve | Δ vs. Primary | $ Target | % |
|---|---|---|---|---|
| ISRG | Mansion | +$10K | $60,000 | 12.0% |
| NVDA | Mansion | -$10K (de-risk valuation) | $40,000 | 8.0% |
| ABBNY | Mansion | +$5K | $47,000 | 9.4% |
| SIEGY | Mansion | +$5K | $47,000 | 9.4% |
| KEYS | Mansion | unchanged | $40,000 | 8.0% |
| CGNX | Mansion | -$3K | $35,000 | 7.0% |
| FANUY | Mansion | -$3K | $35,000 | 7.0% |
| ROK | Middle | unchanged | $18,000 | 3.6% |
| ADI | Middle | +$2K | $20,000 | 4.0% |
| TER | Middle | -$2K | $16,000 | 3.2% |
| MPWR | Middle | unchanged | $15,000 | 3.0% |
| AXON | Middle | -$2K | $13,000 | 2.6% |
| NXPI | Middle | -$3K | $12,000 | 2.4% |
| ZBRA | Middle | unchanged | $11,000 | 2.2% |
| HON | Middle | unchanged | $10,000 | 2.0% |
| SYM | Satellite | -$2K | $5,000 | 1.0% |
| AVAV | Satellite | -$2K | $4,000 | 0.8% |
| ALGM | Satellite | -$1K | $4,000 | 0.8% |
| HSAI | Satellite | -$1K | $4,000 | 0.8% |
| KTOS | Satellite | unchanged | $4,000 | 0.8% |
| SERV | Satellite | removed | — | — |
| CASH | Cash | +$10K | $60,000 | 12.0% |
| **TOTAL** | | | **$500,000** | **100.0%** |

Constraints: Mansion $304K (7 pos), Middle $115K (8 pos), Satellite $21K (5 pos at floor), Cash 12.0% at ceiling. ✓

---

## 10. Exposure by Subsector — Primary Portfolio

| Subsector | $ Exposure | % of Portfolio | Tickers |
|---|---|---|---|
| Surgical robotics | $50,000 | 10.0% | ISRG |
| Robot brain / simulation | $50,000 | 10.0% | NVDA |
| Industrial automation incumbents | $102,000 | 20.4% | ABBNY, SIEGY, ROK |
| Test & measurement | $58,000 | 11.6% | KEYS, TER |
| Sensing / perception | $61,000 | 12.2% | CGNX, ADI, HSAI |
| Robotics OEMs | $38,000 | 7.6% | FANUY |
| Power management | $15,000 | 3.0% | MPWR |
| Embedded compute (non-NVDA) | $15,000 | 3.0% | NXPI |
| Defense / public-safety autonomy | $25,000 | 5.0% | AXON, AVAV, KTOS |
| Warehouse / logistics | $28,000 | 5.6% | ZBRA, HON, SYM |
| Motion / actuation (silicon) | $5,000 | 1.0% | ALGM |
| Last-mile / consumer autonomy | $3,000 | 0.6% | SERV |
| Cash | $50,000 | 10.0% | — |
| **TOTAL** | **$500,000** | **100.0%** | |

**Notes on subsector classifications:**
- ADI is classified under sensing/perception here for its MEMS IMU dominance, although it has motor-control and power components as well.
- TER is classified under test & measurement here (where its market cap weight resides) but also delivers robotics OEM exposure via UR/MiR. Both classifications are defensible.
- ABBNY is classified under industrial automation incumbents though it is also a top-4 industrial robot OEM.

---

## 11. Correlation and Macro-Risk Analysis

The portfolio looks diversified by subsector but contains several correlated risk factors that compound in a downturn. The honest hidden overlaps:

### 11.1 Industrial-cycle correlation
**Affected positions (~$237K, ~47% of portfolio):** ABBNY, SIEGY, ROK, FANUY, KEYS, CGNX, NXPI, HON, ZBRA, TER, ADI, MPWR.
**Risk:** A global manufacturing PMI rolling below 48 for two quarters historically produces 25–35% drawdowns across industrial automation names. This is the single largest correlated risk in the portfolio.

### 11.2 Geographic concentration
- **Japan (~$38K direct + Japan-driven supply chain):** FANUY directly; indirect exposure to Japanese motion-control names via Cognex's customer base.
- **Germany / EU (~$42K direct):** SIEGY directly; ABBNY (Swiss but EU-customer-heavy) effectively another ~$42K, putting Europe at ~$84K (~17%).
- **China revenue exposure (indirect, ~$130K weighted):** Fanuc ~30% of sales, ABB ~15%, Siemens ~15%, NVDA datacenter restrictions, NXPI ~25%, ADI ~20%, Cognex ~20%, Keysight ~15%, MPWR ~50% (China is MPWR's largest revenue geography). A China industrial slowdown or export-control escalation is a real cluster risk.
- **US-heavy positions:** ROK, AXON, SYM, KTOS, AVAV, ISRG, NVDA, TER, ZBRA, HON, HSAI (US-listed Chinese — political tail risk).

### 11.3 Capex cyclicality
EV/battery and semis capex have been the largest swing drivers for ABBNY, SIEGY, FANUY, KEYS, CGNX, ROK, MPWR. A simultaneous EV downcycle + semis trough (we saw this in 2023–24) would drawdown a meaningful slice of the portfolio in lockstep.

### 11.4 Datacenter AI correlation
NVDA is by far the largest datacenter-AI-correlated position (~10%). The mandate is to *not* run a datacenter AI portfolio — and the portfolio does not — but NVDA cannot be excluded without abandoning the dominant robotics-software thesis. If datacenter AI cycle peaks, expect mark-to-market drawdown on NVDA disconnected from the robotics fundamentals.

### 11.5 Robot hype cycle risk
**Affected:** SYM, HSAI, AVAV, KTOS, SERV, NVDA (partial), Cognex (partial), Symbotic (heavily).
A "humanoid winter" — i.e., a year in which the consensus narrative shifts from "humanoids are imminent" to "humanoids are decades away" — could compress the satellite sleeve by 40–60% and put indirect pressure on NVDA and Cognex via robotics-narrative deflation. The satellite sleeve is sized (6.4%) so this is survivable.

### 11.6 Defense budget risk
AVAV, KTOS, AXON have direct US defense/public-safety budget sensitivity. A continuing-resolution scenario or major program reshuffle is real near-term risk.

### 11.7 Automotive cycle risk
NXPI, ADI, ALGM, MPWR, ON (not held), Keysight, CGNX — all have meaningful auto exposure. An auto inventory destocking cycle (we are still recovering from one) is a correlated risk.

### 11.8 Surgical-procedure recession risk
ISRG benefits from elective-procedure volume; a deep US recession or hospital-capex freeze would weigh on ISRG. Historically resilient but not zero.

**Net assessment:** The single largest correlated risk is **global industrial cycle + China industrial slowdown + EV capex pause** simultaneously hitting roughly 50% of the book. The portfolio is structured to ride that risk because the underlying franchises (Fanuc, Siemens, ABB, Cognex, Keysight) have all survived prior cycles intact and emerged share-gainers. But the drawdown risk on a 2-year horizon is real — *do not own this portfolio if you cannot tolerate a 25–30% peak-to-trough mark.*

---

## 12. What Could Break the Thesis — Disconfirming Evidence

Concrete things to watch for that would falsify the Physical AI investment thesis as constructed here:

1. **Humanoid BOM does not fall.** If actuator costs (particularly harmonic reducers and frameless torque motors) do not fall by 50%+ by 2028, humanoid economics never close at any meaningful labor-substitution use case. *Watch:* Harmonic Drive Systems (6324.T) and Nabtesco (6268.T) margin trends — *rising* component prices imply tight supply and no cost-down curve; *flat* prices imply scaling stalled; *falling* prices imply the curve is working.

2. **VLA models plateau.** If the next generation of Physical-Intelligence-class VLA models (after π-0.5) does not show step-function dexterity gains, the entire "general-purpose robot" thesis stalls. The robotics narrative deflates and the satellite sleeve compresses materially.

3. **NVIDIA loses the robotics platform.** If a competitor (Qualcomm, AMD/Xilinx, an open-source RISC-V stack, or a hyperscaler captive design) captures meaningful robot-brain socket share by 2028, NVDA's mansion-grade Physical AI thesis weakens (datacenter thesis is separate).

4. **Open-source VLA + open-source ROS dominates.** If a credible open-source VLA + Isaac-replacement gains traction with industrial OEMs, the software profit pool that NVDA was supposed to compound on never materializes.

5. **Industrial automation incumbents are disintermediated.** If a credible greenfield PLC + edge-AI vendor takes >5% market share by 2030 in either North America or Europe, the Siemens/Rockwell/ABB moat thesis is at risk. (We assess this probability as low — the integrator network is a deeper moat than the silicon — but worth watching.)

6. **Surgical-robot competition intensifies materially.** If Medtronic Hugo or J&J Ottava take >10% of the soft-tissue market by 2028 *and* compress ISRG's pricing power on consumables, the ISRG mansion thesis weakens.

7. **Symbotic-Walmart relationship reprices.** If Walmart slows or renegotiates the deployment cadence, SYM rerates 40%+ down. (Risk-managed via satellite sizing.)

8. **Defense procurement reshuffle.** A major shift in US Replicator / Tactical Autonomy funding could hit AVAV/KTOS materially.

9. **China retaliation / export-control acceleration.** A coordinated Chinese restriction on rare-earth magnets or precision-gear exports could compress the supply chain for ABBNY, FANUY, Yaskawa, Tesla Optimus, and every humanoid OEM globally. This is the most painful tail risk to monitor.

10. **A genuine humanoid winner emerges publicly.** If Figure, Apptronik, or 1X IPOs at sub-stratospheric multiples *and* shows real per-unit gross margins, the *component-supplier-only* thesis weakens because the OEMs themselves become investable. This is a *good* scenario for the world but would require portfolio rebalancing.

---

## 13. One-Page Buy List

| Sleeve | Ticker | $ Target |
|---|---|---|
| **Mansion** | ISRG | $50,000 |
| **Mansion** | NVDA | $50,000 |
| **Mansion** | ABBNY | $42,000 |
| **Mansion** | SIEGY | $42,000 |
| **Mansion** | KEYS | $40,000 |
| **Mansion** | CGNX | $38,000 |
| **Mansion** | FANUY | $38,000 |
| **Middle** | ROK | $18,000 |
| **Middle** | ADI | $18,000 |
| **Middle** | TER | $18,000 |
| **Middle** | MPWR | $15,000 |
| **Middle** | AXON | $15,000 |
| **Middle** | NXPI | $15,000 |
| **Middle** | ZBRA | $11,000 |
| **Middle** | HON | $10,000 |
| **Satellite** | SYM | $7,000 |
| **Satellite** | AVAV | $6,000 |
| **Satellite** | ALGM | $5,000 |
| **Satellite** | HSAI | $5,000 |
| **Satellite** | KTOS | $4,000 |
| **Satellite** | SERV | $3,000 |
| **Cash** | — | $50,000 |
| **TOTAL** | | **$500,000** |

---

## Closing note

If Physical AI becomes a major investable wave over the next decade, public-market investors will most likely make money in:
1. **The surgical-robotics monopoly (ISRG).**
2. **The motion-control + automation incumbents (Fanuc, ABB, Siemens, Yaskawa, Rockwell).**
3. **Picks-and-shovels component suppliers (NVIDIA Jetson, Cognex, ADI, MPWR, Allegro, NXPI).**
4. **Selective defense autonomy** (AVAV, KTOS, Anduril if/when public).
5. **The warehouse automation incumbents** (Symbotic — sized carefully — and the broader Honeywell/Zebra/Dematic stack).

They will *probably not* make money buying generic humanoid OEM stories at 2024–2026 vintage valuations. The single best protection against the humanoid hype cycle is to own the layers humanoids cannot exist without — and let the OEMs prove their economics on someone else's capital.

— *End of report.*
