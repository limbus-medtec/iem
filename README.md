# IEM Configuration
This repository contains configuration files for the Illumina® Experiment Manager (IEM) for third-party indices. Adding these files to your IEM configuration will allow you to create SampleSheets using IEM for third-party library kits.

The configuration files were created for use with IEM 1.18.1 following the instructions in the [IEM Software Guide](https://emea.support.illumina.com/content/dam/illumina-support/documents/documentation/software_documentation/iem/illumina-experiment-manager-software-guide-15031335-08.pdf) from December 2018.

The files are provided as a courtesy to users of the [varvis® software](https://www.varvis.com). They are free to use for anybody else. Feedback or feature requests are always welcome.

## Disclaimer

The configuration files are provided "as is" and the authors make no representations or warranties of any kind concerning suitability, correctness or functionality. These files are not part of the medical device [varvis®](https://www.varvis.com).

Links to other websites are provided as a convenience and do not indicate any endorsement or business relationship.

## Installation

IEM is typically installed into a directory such as this:

```
C:\Program Files (x86)\Illumina\Illumina Experiment Manager
```

The IEM program directory contains four directories:

```
Applications
Genomes
IndexKits
SamplePrepKits
```

Copy the files from the directories in this repository into the respective directory of IEM on your computer. Then, restart IEM. 

> Note that you will probably need administrator rights on your computer in order to modify files in the program directory.

## Integrated DNA Technologies

The following IDT adapters are contained in the configuration files.

### xGen® Dual Index UMI Adapters (8nt)

www.idtdna.com/UMI-techaccess

384 unique dual index adapters are grouped into four sets of 96 adapters. 

> Note that the index sequences in this configuration do not contain `N` for UMI nucleotides, since [varvis®](https://www.varvis.com) takes care of separation of barcode sequences.

## Twist Bioscience Universal Adapter System

The datasheet of the Twist unique dual index adapters is available here: https://www.twistbioscience.com/resources/twist-universal-adapter-system

### 16-UDI

16 unique dual index adapters.

### 96-UDI

384 unique dual index adapters are grouped into four sets of 96 adapters. 

Illumina® is a registered trademark of Illumina, Inc. xGen® is a registered trademark of Integrated DNA Technologies, Inc. All other trademarks are property of their respective owners.