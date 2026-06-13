# ![SabreTools Organization Logo](images/sabretools-rect-new-transparent.svg)

Welcome to the SabreTools family of projects! Below you can learn about the various projects under the SabreTools umbrella, including links to each. SabreTools projects are maintained by [mnadareski](https://github.com/mnadareski) with contributions by many dedicated developers and hobbyists.

Projects generally use the **MIT License** and all serious contributions are welcome. All projects that utilize C\# are designed to be as broadly compatible across .NET versions as possible, often stretching as old as **.NET Framework 2.0**.

The SabreTools program logo was designed by **Kludge** and the current organization logo was designed by [**Whatever Industries**](https://github.com/whatev-indus). Both are used with permission in their respective contexts.

---
---

## Programs

The SabreTools family of projects includes multiple programs that are designed to fit some very specific niches, often in the realm of media preservation and data processing. Most of the programs below are commandline applications, with the exception of the UI components of **MPF**.

### [Media Preservation Frontend](https://github.com/SabreTools/MPF)

**Media Preservation Frontend**, or just **MPF**, is the defacto disc dumping frontend used by [Redump](http://redump.org/) and related communities. It offers multiple user-friendly options to work with various disc dumping programs, such as [redumper](https://github.com/superg/redumper), [Aaru](https://github.com/aaru-dps/Aaru), and [DiscImageCreator](https://github.com/saramibreak/DiscImageCreator).

Included in the repo there are 4 applications:

- **MPF.UI** is the main GUI application for MPF. It is written using WPF as the UI framework so it is Windows-specific. It provides many features including media dumping, checking of existing output files, and IRD creation.

- **MPF.Avalonia** is a work-in-progress cross-platform GUI application for MPF. It is written using Avalonia as the UI framework, allowing for Windows, Linux, and Mac vresions. When completed, it will provide many features including media dumping, checking of existing output files, and IRD creation.

- **MPF.CLI** is the commandline equivilent to **MPF.UI**. It allows for users to take advantage of the dumping and post-dump processing steps from the terminal instead. The application also includes an interactive mode for users who are uncomfortable with commandline flags. It is fully cross-platform, with builds available for Windows, Linux, and Mac.

- **MPF.Check** is a standalone application allowing users to check existing output files. It is useful for processing the outputs from some non-desktop applications such as CleanRip. The application also includes an interactive mode for users who are uncomfortable with commandline flags. It is fully cross-platform, with builds available for Windows, Linux, and Mac.

### [NDecrypt](https://github.com/SabreTools/NDecrypt)

**NDecrypt** is an easy-to-use Nintendo DS and 3DS encryption and decryption tool. Users must provide their own legally-obtained keys and data. Additional information output for verifying the transformed files is also included. It originally was fully separated from other projects, but now utilizes **SabreTools.IO** and **SabreTools.Serialization** instead.

### [SabreTools](https://github.com/SabreTools/SabreTools)

**SabreTools** is the flagship and origination of the entire family of projects. It is a highly-advanced metadata file creation and manipulation tool aimed at users who know their way around a command line. The associated [wiki](https://github.com/SabreTools/SabreTools/wiki) is one the most thorough set of documents on the various metadata formats that exist out in the wild.

### [UnshieldSharp](https://github.com/mnadareski/UnshieldSharp)

**UnshieldSharp** is a standalone application designed to extract InstallShield Cabinet files. It originated as a C\# port of [Unshield](https://github.com/twogood/unshield/), now utilizes **SabreTools.Serialization** instead. This program is not officially part of the SabreTools family of projects, but is highly coupled to it.

### [WiseUnpacker](https://github.com/mnadareski/WiseUnpacker)

**WiseUnpacker** is a standalone application designed to extract Wise Installer executables. It originated as a C\# port of both [E_WISE](https://kannegieser.net/veit/quelle/index_e.htm) and [Heuristic Wise-Setup Unpacker (HWUN)](http://www.angelfire.com/ego/jmeister/hwun/). The current implementation is based on work done for [REWise](https://codeberg.org/CYBERDEV/REWise) which utilizes **SabreTools.Serialization** instead. This program is not officially part of the SabreTools family of projects, but is highly coupled to it.

---
---

## Libraries

Libraries make up the bulk majority of the projects included under the SabreTools banner. These projects are well-maintained and continue to evolve over time. Many of the libraries include at least one reference implementation program that is designed to show off various pieces of functionality.

### [BinaryObjectScanner](https://github.com/SabreTools/BinaryObjectScanner)

**BinaryObjectScanner**, formerly **BurnOutSharp**, is a comprehensive protection scanning library. It can detect dozens of protections and packers, including in many common compressed formats. It is supported by its sibling research project, [DRML](https://github.com/TheRogueArchivist/DRML).

Included in the repo is a standalone application called **ProtectionScan**, which acts as a reference for anyone who wishes to incorporate **BinaryObjectScanner** in their projects.

### [SabreTools.CommandLine](https://github.com/SabreTools/SabreTools.CommandLine)

**SabreTools.Commandline** is a utility library designed as an alternative to other commandline processing solutions. It intends to be extensible and flexible enough to support even the most complicated commandline flag combinations. It is used heavily by the various commandline applications across the family of projects.

### [SabreTools.Hashing](https://github.com/SabreTools/SabreTools.Hashing)

**SabreTools.Hashing** is a library that provides a uniform experience for implementers who need checksum and hash processing. It supports a broad range of options, many of which are written in fully-managed C\#.

Included in the repo is a standalone application called **Hasher**, which acts as a reference for anyone who wishes to incorporate **SabreTools.Hashing** in their projects.

### [SabreTools.IO](https://github.com/SabreTools/SabreTools.IO)

**SabreTools.IO** is a comprehensive meta-library that acts as the primary utility library for many of the other SabreTools projects. It includes numerous extensions as well as compression and encryption functionality. Please see the per-project README files for a much more thorough look into what the meta-library is capable of.

### [SabreTools.RedumpLib](https://github.com/SabreTools/SabreTools.RedumpLib)

**SabreTools.RedumpLib** is a reference library used to document and interact with the [Redump](http://redump.org/) website. No formal API exists for the current site, so this acts as a psuedo-API layer. It is primarily used by **MPF** to help retrieve match data.

Included in the repo is a standalone reference application called **RedumpTool**, which allows for programmatic access to the site, including the ability to supply login credentials for locked functionality.

### [SabreTools.Serialization](https://github.com/SabreTools/SabreTools.Serialization)

**SabreTools.Serialzation** is a comprehensive meta-library that acts the primary file processing library for many of the other SabreTools projects. It includes dozens of file models, readers, writers, custom information wrappers, as well as metadata file management.

Included in the repo there are 2 reference applications:

- **ExtractionTool** provides an easy-to-use commandline method of using the extraction capabilities of both **SabreTools.IO** and **SabreTools.Serialization**. It acts as a reference for anyone looking to incorporate the unique extraction functionality in their own programs.

- **InfoPrint** allows users to generate comprehensive reports about the structure of the dozens of supported file formats. It provides both a human-readable textfile output as well as an optional machine-parseable JSON output. It acts as a reference for anyone looking to incorporate the custom wrapper functionality in their own programs.

### [SabreTools.Skippers](https://github.com/SabreTools/SabreTools.Skippers)

**SabreTools.Skippers** is a utility library meant to help deal with the various header skipper definitions that exist. Header skippers were traditionally distributed as XML definition files and used by various file management programs.

Included in the repo is a standalone program called **Headerer** which allows users to remove and restore copier headers from various supported formats.

---
---

## Unmaintained and Retired Projects

Some projects under the umbrella of the SabreTools family are considered to be unmaintained or archived for one reason or another. Any archived projects that were merged into one of the maintained libraries are not listed here. Below are a list of those projects along with their original purpose.

### [psxt001z](https://github.com/SabreTools/psxt001z)

**psxt001z** is a mostly-unmaintained C\# port of [psxt001z](https://github.com/Dremora/psxt001z). It does not surface all of the same direct-disc functionality that the original tool did, instead focusing on just subchannel processing.

### [Reheader](https://github.com/SabreTools/Reheader)

**Reheader** was an experimental application that used a Mesen database file to regenerate iNES 2.0 headers for cart images. It has not been touched in many years due to a lack of community interest.

### [Transform](https://github.com/SabreTools/Transform)

**Transform** was originally an application designed to experiment with various methods of transforming input files. The majority of the functionality that was included here is now in **SabreTools.IO**. This program is kept around as a standalone implementation but should not be relied on anymore.

### [TwoFour](https://github.com/SabreTools/TwoFour)

**TwoFour** was a utility application that allowed converting data stores that used [romba](https://github.com/uwedeportivo/romba) organization to different, configurable depths. 4 levels has since been standardized, rendering this application unneeded.

### [Wizard of DATz Redux](https://github.com/SabreTools/wizzardRedux)

**Wizard of DATz (WoD) Redux** was a PHP application that was meant to aid in documenting available files across a large variety of sources. The code was originally written and maintained by **Wizard of DATz (WoD)**. This project formed the basis of what became the **SabreTools** commandline application.

---
---
