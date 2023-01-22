# Version 0.13.0 (2023-01-22)

## API

- Add `FileFormat::short_name`
- Improve crate features
- Change the media type of Adobe Illustrator Artwork (AI) to `application/vnd.adobe.illustrator`

## Docs

- Improve global documentation

## Fixes

- Fix LHA signatures
- Fix vCalendar (VCS) extension

## Internal changes

- Improve the detection of Extensible Markup Language (XML) based file formats
- Move the declaration of the file formats to a dedicated module

## New formats support

- Extensible 3D Graphics (X3D)
- GPS Exchange Format (GPX)
- LArc (LZS)
- PMarc (PMA)
- XML Localization Interchange File Format (XLIFF)
- iCalendar (ICS)

# Version 0.12.0 (2022-12-30)

## API

- Add `accuracy` feature

## Docs

- Improve global documentation
- Simplify `lefi` example

## New formats support

- LaTeX (TeX)

# Version 0.11.0 (2022-12-21)

## Docs

- Remove dependencies of `lefi` example

## New formats support

- Clojure Script
- Extensible Markup Language (XML)
- Extensible Stylesheet Language Transformations (XSLT)
- Geography Markup Language (GML)
- HyperText Markup Language (HTML)
- Keyhole Markup Language (KML)
- Lua Script
- MusicXML
- MusicXML Zipped (MXL)
- Perl Script
- Plain Text (TXT)
- Python Script
- Really Simple Syndication (RSS)
- Ruby Script
- Scalable Vector Graphics (SVG)
- Shell Script
- Simple Object Access Protocol (SOAP)
- Tool Command Language Script
- vCalendar (VCS)
- vCard (VCF)

# Version 0.10.0 (2022-12-04)

## Fixes

- Fix inverted names between `MatroskaVideo` and `MetaInformationEncapsulation`

## New formats support

- Common Object File Format (COFF)
- Google Draco (Draco)
- ICC Profile (ICC)
- Mach-O
- OpenRaster (ORA)

# Version 0.9.1 (2022-11-30)

## Docs

- Fix `README.md`

# Version 0.9.0 (2022-11-30)

## API

- Add `FileFormat::kind`
- Rename `AdobeInDesignDocument` to `AdobeIndesignDocument`
- Rename `Ani` to `WindowsAnimatedCursor`
- Rename `AppleQuickTime` to `AppleQuicktime`
- Rename `Cur` to `WindowsCursor`
- Rename `EmbeddedOpenType` to `EmbeddedOpentype`
- Rename `Ico` to `WindowsIcon`
- Rename `JavaKeyStore` to `JavaKeystore`
- Rename `MacOsAlias` to `MacosAlias`
- Rename `MicrosoftVisioDrawing` to `OfficeOpenXmlDrawing`
- Rename `MpegAudioLayer3` to `Mpeg12AudioLayer3`
- Rename `OfficeOpenXmlWorkbook` to `OfficeOpenXmlSpreadsheet`
- Rename `OpenExr` to `Openexr`
- Rename `OpenType` to `Opentype`
- Rename `ScreamTracker3Module` to `Screamtracker3Module`
- Rename `SeqBox` to `Seqbox`
- Rename `SketchUp` to `Sketchup`
- Rename `TrueType` to `Truetype`
- Rename `VirtualBoxVirtualDiskImage` to `VirtualboxVirtualDiskImage`
- Rename `WavPack` to `Wavpack`
- Rename `WebAssemblyBinary` to `WebassemblyBinary`
- Rename `WebP` to `Webp`
- Rename `WindowsExecutable` to `MsDosExecutable`
- Rename `XpInstall` to `Xpinstall`

## Fixes

- Add MPEG-1/2 Audio Layer 3 (MP3) signature
- Add Matroska Video (MKV) signature
- Change UNIX archiver extension from `ar` to `a` (preferred)
- Fix Apple QuickTime (MOV) signature
- Fix Joint Photographic Experts Group (JPEG) signature

## Internal changes

- Add `formats` macro
- Split items into modules

## New formats support

- Adobe Illustrator Artwork (AI)
- Circuit Diagram Document (CDDX)
- Creative Voice (VOC)
- DER Certificate (DER)
- DjVu
- Dynamic Link Library (DLL)
- Encapsulated PostScript (EPS)
- Enterprise Application Archive (EAR)
- Keyhole Markup Language Zipped (KMZ)
- LLVM Bitcode (BC)
- Lua Bytecode
- MPEG-1 Audio Layer 1 (MP1)
- MPEG-1 Audio Layer 2 (MP2)
- MPEG-2 Transport Stream (MTS)
- Meta Information Encapsulation (MIE)
- Microsoft Access 2007 Database (ACCDB)
- Microsoft Access Database (MDB)
- Microsoft Excel Spreadsheet (XLS)
- Microsoft PowerPoint Presentation (PPTX)
- Microsoft Project Plan (MPP)
- Microsoft Publisher Document (PUB)
- Microsoft Software Installer (MSI)
- Microsoft Visio Drawing (VSD)
- Microsoft Word Document (DOC)
- PEM Certificate (CRT)
- PEM Certificate Signing Request (CSR)
- PEM Private Key (KEY)
- PGP Message (ASC)
- PGP Private Key Block (ASC)
- PGP Public Key Block (ASC)
- PGP Signature (ASC)
- PGP Signed Message (ASC)
- Portable Executable (PE)
- PostScript (PS)
- Rich Text Format (RTF)
- Sony Movie (MQV)
- TASTy
- Web Application Archive (WAR)
- WebM
- Windows App Package (APPX)
- iOS App Store Package (IPA)

# Version 0.8.0 (2022-11-06)

## API

- Add `FileFormat::from_reader`
- Add `impl From<&[u8]> for FileFormat`

## Docs

- Add `lefi` example
- Add `CHANGELOG.md`

## Internal changes

- Make signature offset optional
- Remove `FileFormat` enum generation with macro
- Simplify `signatures` macro

## New formats support

- 3D Manufacturing Format (3MF)
- Android Package (APK)
- Design Web Format XPS (DWFX)
- Electronic Publication (EPUB)
- Java Archive (JAR)
- Microsoft Visio Drawing (VSD)
- Microsoft Visual Studio Extension (VSIX)
- Office Open XML Document (DOCX)
- Office Open XML Presentation (PPTX)
- Office Open XML Spreadsheet (XLSX)
- OpenDocument Graphics (ODG)
- OpenDocument Presentation (ODP)
- OpenDocument Spreadsheet (ODS)
- OpenDocument Text (ODT)
- XAP
- XPInstall (XPI)

# Version 0.7.0 (2022-08-22)

## New formats support

- Android Binary XML (AXML)
- Android Compiled Resources (ARSC)
- Optimized Dalvik Executable (DEY)

# Version 0.6.0 (2021-12-18)

## API

- Add `FileFormat::from_bytes`

# Version 0.5.0 (2021-12-12)

## API

- Switch back `FileFormat` type from a structure to an enum

## Discontinued formats

- 3D Manufacturing Format (3MF)
- Java Archive (JAR)
- MPEG-2 Transport Stream (MTS)
- Microsoft Visio Drawing (VSD)
- Office Open XML Document (DOCX)
- Office Open XML Presentation (PPTX)
- Office Open XML Spreadsheet (XLSX)
- OpenDocument Graphics (ODG)
- OpenDocument Presentation (ODP)
- OpenDocument Spreadsheet (ODS)
- OpenDocument Text (ODT)
- Web Application Resource (WAR)
- XAP
- XPInstall (XPI)

## Improvements

- Add precision to the Dalvik Executable (DEX) signature
- Switch to Rust 2021

## New formats support

- Java KeyStore (JKS)

# Version 0.4.0 (2021-10-22)

## Docs

- Reorganize supported file formats table

## Improvements

- Add tests for all High Efficiency Image Coding Sequence (HEICS) format
- Add tests for all High Efficiency Image Coding (HEIC) format

## New formats support

- 3D Manufacturing Format (3MF)
- Java Archive (JAR)
- Microsoft DirectDraw Surface (DDS)
- Microsoft Visio Drawing (VSD)
- Office Open XML Document (DOCX)
- Office Open XML Presentation (PPTX)
- Office Open XML Spreadsheet (XLSX)
- Radiance HDR (HDR)
- Web Application Resource (WAR)
- XAP
- XPInstall (XPI)

# Version 0.3.0 (2021-10-18)

## API

- Switch `FileFormat` type from an enum to a structure

## Discontinued formats

- HyperText Markup Language (HTML)

## Fixes

- Use of the correct Tag Image File Format (TIFF) extension

## Improvements

- Add new Apple QuickTime (MOV) signatures
- Add new Audio Interchange File Format (AIFF) signature
- Add precision to the Debian Binary Package (DEB) signature
- Add precision to the Flexible Image Transport System (FITS) signature
- Add precision to the Windows Media Video (WMV) signature
- Add precision to the Windows Shortcut (LNK) signature
- Improve support of some file formats
- Replace Microsoft Software Installer (MSI) by Compound File Binary (CFB)

## New formats support

- ALZ
- Adobe Flash Player Audio (F4A)
- Adobe Flash Player Audiobook (F4B)
- Apache Arrow Columnar (Arrow)
- Apple iTunes Audiobook (M4B)
- Canon Raw 2 (CR2)
- Canon Raw 3 (CR3)
- FastTracker 2 Extended Module (XM)
- Fujifilm Raw (RAF)
- Impulse Tracker Module (IT)
- LHA
- Lempel–Ziv Finite State Entropy (LZFSE)
- Microsoft Compiled HTML Help (CHM)
- Microsoft Virtual Hard Disk (VHD)
- Microsoft Virtual Hard Disk 2 (VHDX)
- Nikon Electronic File (NEF)
- Panasonic Raw (RW2)
- Qualcomm PureVoice (QCP)
- ScreamTracker 3 Module (S3M)
- SeqBox (SBX)
- Snappy
- Sony DSD Stream File (DSF)
- Windows Animated Cursor (ANI)
- Windows Cursor (CUR)
- cpio
- macOS Alias (Alias)
- zoo

# Version 0.2.1 (2021-10-14)

## Fixes

- Fix Tag Image File Format (TIFF) signature

# Version 0.2.0 (2021-10-07)

## New formats support

- Animated Portable Network Graphics (APNG)
- Electronic Publication (EPUB)
- Game Boy Color ROM (GBC)
- HyperText Markup Language (HTML)
- Khronos Texture (KTX)
- Khronos Texture 2 (KTX2)
- MPEG-2 Transport Stream (MTS)
- Material Exchange Format (MXF)
- Mobipocket (MOBI)
- Olympus Raw Format (ORF)
- OpenDocument Graphics (ODG)
- OpenDocument Presentation (ODP)
- OpenDocument Spreadsheet (ODS)
- OpenDocument Text (ODT)
- Rich Text Format (RTF)
- Shapefile (SHP)
- SketchUp (SKP)
- UNIX archiver

# Version 0.1.0 (2021-10-03)

First version.