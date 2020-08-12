---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Autumn Naber
---
## Highlights
* **C/C++, Python, Java SE/EE, Bash, Web Dev**, Assembly, Perl, TCL, Verilog/VHDL, SQL
* **SAS/SATA, JTAG, TCP/IP, Regressions, Drivers, Embedded, DSP, ML**, FPGA, RTOS, NVMe
* **Agile/Scrum Development**, Coverage Analysis, Project Advising

## Employment

**Chalmers University of Technology – Research Engineer 2017-2020**
* Develop real-time signal processing and pattern recognition on embedded systems
* Support Bluetooth, WiFi, and serial communication in C, Python, and MATLAB
* Develop PCBs for muscle signal (EMG) acquisition, processing, and transmission
* Develop MATLAB interfaces and GUIs for medical signal acquisition and processing
* Scientific and technical advising of Bachelor’s and Master’s thesis projects
* Teaching: Analog Electronics, Electric Circuits and Fields, Biomedical Instrumentation

**Validation Engineer (Short Contract), Oakgate Technology, California – 2016**
* Customer facing SAS/SATA validation code showcasing full-coverage validation suite

**Software/Validation Engineer, PMC Sierra, California – 2011-2015**
* Java GUI development for interfacing with SAS controller firmware and targets
* Nightly build and regression implementation and maintenance (using SVN and Git)
* Linux diagnostics and validation driver for SAS/SATA HBAs and targets
* Development of flexible Linux virtual SAS target driver with error injection
* Work with JTAG probes and SAS analyzers for firmware debugging

**System Support, California State University, Sacramento – 2009-2011**
* Enterprise-level network management with HP and Juniper products
* Remote software and OS deployment, administration, and maintenance

## Education

**Chalmers University of Technology – M.S. Biomedical Engineering (2017)**
* Applied signal processing and machine learning for medical instrumentation
* Computational electromagnetics and complex systems modelling and simulation
* Thesis: “Stationary wavelet processing and data imputing in myoelectric pattern
recognition on a low-cost embedded system.", 2019, IEEE TMRB

**California State University, Sacramento – B.S. Computer Engineering (2013)**
* Minor in mathematics focussing on numerical optimization
* Design and build of a multi-threaded operating system in C and Intel Assembly
* VHDL design of full multi-path MIPS CPU and PCI-compatible SRAM memory module
* Finalist entry at I2P Biotechnology Symposium for thesis work
* Thesis: Device to optimize tissue survival rate for transplants in humans

## Publications

Abbaspour, Sara, et al. "Evaluation of surface EMG-based recognition algorithms for decoding hand movements." Medical & Biological Engineering & Computing 58.1 (2020): 83-100.

Naber, Autumn, Enzo Mastinu, and Max Ortiz-Catalan. "Stationary Wavelet Processing and Data Imputing in Myoelectric Pattern Recognition on a Low-Cost Embedded System." IEEE Transactions on Medical Robotics and Bionics 1.4 (2019): 256-266.

Ortiz-Catalan, Max, et al. "Patterned stimulation of peripheral nerves produces natural sensations with regards to location but not quality." IEEE Transactions on Medical Robotics and Bionics 1.3 (2019): 199-203.

Naber, A., Yiannis Karayiannidis, and Max Ortiz-Catalan. "Universal, Open Source, Myoelectric Interface for Assistive Devices." 2018 15th International Conference on Control, Automation, Robotics and Vision (ICARCV). IEEE, 2018.

Maier, Julian, Adam Naber, and Max Ortiz-Catalan. "Improved prosthetic control based on myoelectric pattern recognition via wavelet-based de-noising." IEEE Transactions on Neural Systems and Rehabilitation Engineering 26.2 (2017): 506-514.

## Projects

### LiPo-Powered Wireless Communication Solution for EMG Acquisition

**Chalmers University of Technology. 2020**

**Overview**
The open-source !ADS_BP electromyography acquisition hardware suffered from
significant limitation from the power supply and Bluetooth communications.
A custom, low-noise board was produced with updated firmware to dramatically
enhance the portability, useability, and reliability of the device.

**Responsibilities**
* Design and prototype single PCB for low-noise power supply and WiFi communications
* Design and prototype updated PCB for !ADS_BP module with improved electrode connections
* Implement error-tolerant, wireless DFU-enabled bootloader
* Open-source code and hardware - Coming Soon

### Surface EMG Noise Suppression via Wavelet Transform

**Chalmers University of Technology. Journal Publication. 2019**

**Overview**
Electromyography signals read from non-invasive surface electrodes (like those
used for heart monitoring) is often noisy, susceptible to mechanical 
interference from movement, and loss of electrode contace. Algorithms were 
designed and implemented to address each issue and tested on human subjects
within an appropriate ethical framework.

**Responsibilities**
* Design and implement MCU-compatible wavelet transform and reconstruction (C)
* Implement signal denoising, artifact reduction, and data imputing routines (C)
* Data collection, interpretation, and visualization (MATLAB/Python)
* Journal publication - [Link](https://doi.org/10.1109/tmrb.2019.2949853)
* Open-source code - [Link](https://github.com/casualformality/ADS_BP)

### High-Dimensional Data Visualization via Stochastic Mapping

**Chalmers University of Technology. 2018**

**Overview**
Electromyography signals are often read from many different muscle 
simultaneously. When training users to control EMG-driven interfaces, like
prosthetic arms, the signal information needs to be condensed in a manner that
is easy to visually parse. t-Distributed Stochastic Neighborhood Embedding and 
a neural network were used to condense the information from the many features 
over many channels down to 2-dimensions and plotted on a graph in real-time, 
respectively.

**Responsibilities**
* Implement t-SNE mapping and neural network encoding of EMG signals (MATLAB)
* Open-source code - Coming Soon

### EMG Signal Compression

**Chalmers University of Technology. 2018**

**Overview**
Electromyography signals for clinical and research use often need to be sampled
at tens of kHz using multiple channels. As a result, low-power wireless 
solutions often struggle to transmit the necessary data. A low-loss signal
compression algorithms was developed based on Mu-Law companding to reduce the
communication overhead with minimal processing power.

**Responsibilities**
* Implement 16-bit data companding and reconstruction algorithms (C/MATLAB)
* Test and compare 16-bit companding with other algorithms
* Open-source code - Coming Soon

### Semi-Autonomous Quadcopter Control

**Chalmers University of Technology. Conference Paper. 2018**

**Overview**
Pattern recognition can be used translate motor intention, even in cases of 
apparent paralysis from stroke or spinal cord injury, into robotic control 
signals for devices like wheelchairs and quadcopters. However, the lack of fine 
control limits its usefullness. A low-cost modular system was developed to 
provide collision avoidance while allowing high-level control of the vehicle.

**Responsibilities**
* Integrate EMG pattern recognition front-end with wireless-enabled quadcopter (Python/MATLAB)
* Develop simulated quadcopter with collision-detection hardware for testing
* Implement attractor/repellor collision-avoidance system for ArduPilot-enabled devices (Python)
* Conference publication - [Link](https://doi.org/10.1109/ICARCV.2018.8581344)
* Open-source code - [Link](https://github.com/biopatrec/SharedControl)

### SAS/SATA Device Emulation Driver for Linux

**PMC-Sierra, Inc. 2015**

**Overview**
Automated tests for software that depend on physical devices (like hard drives) 
requires both that the drives to be in known good states and that the tests have 
physical media dedicated to them. Emulating hard drives within a driver allows 
for testing of arbitrary storage topologies without dedicated media or physical 
setup.

**Responsibilities**
* Upgrade template block driver to emulate arbitrary storage topologies (C)
* Integrate driver with existing test infrastructure for automated test loading

### Automation of Tissue Conditioning for Transplants

**California State University, Sacramento. BSc Thesis. 2013**

**Overview** 
The success of tissue transplants is limited by cell death due to 
shock from low oxygen concentrations and blood perfusion in the new location. 
Slowly exposing tissue to low-oxygen environments increases tissue viability, 
but is labor intensive and can take many hours. A device was constructed to 
automate the process of mixing and separating saline with different oxygen 
concentrations with tissue.

**Personal Responsibilities**
* Design and assemble PCB to control robotic elements of the device (scale, servos, etc.)
* Design and implement UI on Arduino MEGA for setting mixing parameters and providing feedback (C)

**Team Responsibilities**
* Design self-contained unit for housing device
* Select and integrate parts appropriate for work on human tissue
* Project write-up
