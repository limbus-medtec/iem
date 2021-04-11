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
ZIP archives containing all configuration files are provided there.

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
| [IDX96](https://www.nimagen.com/shop/products/idx96-u01/index-primer-plate-and-nbsp-u01-96-unique-dual-indexes) | [Nimagen](https://www.nimagen.com/)    | 10         | `Nimagen UDI`          | `Nimagen IDX96-U01v3`<br />`Nimagen IDX96-U02v2`<br />`Nimagen IDX96-U03`<br />`Nimagen IDX96-U04`<br />`Nimagen IDX96-U05`<br />`Nimagen IDX96-U06`  |
| [IDX96](https://www.nimagen.com/shop/products/idx96-u01/index-primer-plate-and-nbsp-u01-96-unique-dual-indexes) | [Nimagen](https://www.nimagen.com/)   | 8*         | `Nimagen UDI`          | `Nimagen IDX96-U01v3-8nt`<br />`Nimagen IDX96-U02v2-8nt`<br />`Nimagen IDX96-U03-8nt`<br />`Nimagen IDX96-U04-8nt`<br />`Nimagen IDX96-U05-8nt`<br />`Nimagen IDX96-U06-8nt`   |
| [IDX96](https://www.nimagen.com/shop/products/idx96-u01/index-primer-plate-and-nbsp-u01-96-unique-dual-indexes) | [Nimagen](https://www.nimagen.com/)    | 8*         | `Nimagen UDI`          | `Nimagen IDX96-U01v3-RC-8nt`<br />`Nimagen IDX96-U02v2-RC-8nt`<br />`Nimagen IDX96-U03-RC-8nt`<br />`Nimagen IDX96-U04-RC-8nt`<br />`Nimagen IDX96-U05-RC-8nt`<br />`Nimagen IDX96-U06-RC-8nt` |
| [16-UDI](https://www.twistbioscience.com/resources/twist-universal-adapter-system) | [Twist Bioscience](https://www.twistbioscience.com/)         | 10         | `Twist Enrichment UDI` | `Twist 16 UDI`                                               |
| [96-UDI](https://www.twistbioscience.com/resources/twist-universal-adapter-system) | [Twist Bioscience](https://www.twistbioscience.com/)         | 10         | `Twist Enrichment UDI` | `Twist 384 UDI`<br />`Twist 96 UDI Plate A`<br />`Twist 96 UDI Plate B`<br />`Twist 96 UDI Plate C`<br />`Twist 96 UDI Plate D` |

*Some Nimagen amplicon designs require to use at least 151 cycles for Read 1 and Read 2. This is not compatible with 10nt 
indices on most devices. Nimagen states, however, that their 10nt index plates can be used as 8nt indices. 
For convenience, we created configurations with 8nt from those index plates. Please note that you must
select different configurations depending on your device, for example:
* `Nimagen IDX96-U01-8nt` for the Forward Strand Workflow implemented in MiSeq and NovaSeq (v1.0 reagents),
* `Nimagen IDX96-U01-RC-8nt` for the Reverse Complement Workflow implemented in NextSeq and NovaSeq (v1.5 reagents).

See also the Indexed Sequencing Overview Guide Document #15057455 (v08 Nov 2020).

Illumina® is a registered trademark of Illumina, Inc. All other trademarks are property of their respective owners.