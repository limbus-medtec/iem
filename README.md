# IEM Configuration
This repository contains configuration files for the Illumina® Experiment Manager (IEM) for third-party indices. 
Adding these files to your IEM configuration will allow you to create SampleSheets using IEM for third-party library kits.

The configuration files were created for use with IEM 1.19.1 following the instructions in the 
[IEM Software Guide](https://support.illumina.com/content/dam/illumina-support/documents/documentation/software_documentation/iem/illumina-experiment-manager-software-guide-15031335-09.pdf) 
from January 2021.

The files are provided as a courtesy to users of the [varvis® software](https://www.varvis.com). 
They are free to use for anybody else. Feedback or feature requests are always welcome.

## Disclaimer

The configuration files are provided "as is" and the authors make no representations or warranties of any kind 
concerning suitability, correctness or functionality. These files are not part of the medical device 
[varvis®](https://www.varvis.com).

Links to other websites are provided as a convenience and do not indicate any endorsement or business relationship.

## Download

Please download the latest version from [releases](https://github.com/limbus-medtec/iem/releases/latest). 
We provide .zip files with Windows line endings.

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

Copy the files from the directories in this repository into the respective directory of IEM on your computer. 
Then, restart IEM. 

> Note that you will probably need administrator rights on your computer in order to modify files in the program directory.

## Available index adapters

| Name                                                         | Manufacturer                                                 | Length/ nt | SamplePrepKit          | IndexKits                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ---------- | ---------------------- | ------------------------------------------------------------ |
| [IDX96](https://www.nimagen.com/shop/products/idx96-u01/index-primer-plate-and-nbsp-u01-96-unique-dual-indexes) | [Nimagen](https://www.nimagen.com/)                          | 10         | `Nimagen UDI`          | `Nimagen IDX96-U01`<br />`Nimagen IDX96-U02`                 |
| [16-UDI](https://www.twistbioscience.com/resources/twist-universal-adapter-system) | [Twist Bioscience](https://www.twistbioscience.com/)         | 10         | `Twist Enrichment UDI` | `Twist 16 UDI`                                               |
| [96-UDI](https://www.twistbioscience.com/resources/twist-universal-adapter-system) | [Twist Bioscience](https://www.twistbioscience.com/)         | 10         | `Twist Enrichment UDI` | `Twist 384 UDI`<br />`Twist 96 UDI Plate A`<br />`Twist 96 UDI Plate B`<br />`Twist 96 UDI Plate C`<br />`Twist 96 UDI Plate D` |

Illumina® is a registered trademark of Illumina, Inc. All other trademarks are property of their respective owners.