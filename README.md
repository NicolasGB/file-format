# file-format

![Build](https://img.shields.io/github/workflow/status/mmalecot/file-format/CI)
[![Crates.io](https://img.shields.io/crates/v/file-format.svg)](https://crates.io/crates/file-format)
[![Docs](https://docs.rs/file-format/badge.svg)](https://docs.rs/file-format)
![Rust](https://img.shields.io/badge/rust-1.56+-blueviolet.svg?logo=rust)
![License](https://img.shields.io/badge/license-MIT%2FApache--2.0-blue.svg)

File format library for Rust.

This crate is for determining binary-based file formats.

## Examples

Determines from a file:

```rust
use file_format::FileFormat;

let format = FileFormat::from_file("fixtures/application/sample.zip").unwrap();
assert_eq!(format, FileFormat::Zip);
assert_eq!(format.name(), "ZIP");
assert_eq!(format.media_type(), "application/zip");
assert_eq!(format.extension(), "zip");
```

Determines from bytes:

```rust
use file_format::FileFormat;

let format = FileFormat::from_bytes(&[0xFF, 0xD8, 0xFF, 0xEE]);
assert_eq!(format, FileFormat::JointPhotographicExpertsGroup);
assert_eq!(format.name(), "Joint Photographic Experts Group");
assert_eq!(format.media_type(), "image/jpeg");
assert_eq!(format.extension(), "jpg");
```

## Supported formats

- Adaptive Multi-Rate (amr)
- Adobe Flash Player Audio (f4a)
- Adobe Flash Player Audiobook (f4b)
- Adobe Flash Player Protected Video (f4p)
- Adobe Flash Player Video (f4v)
- Adobe InDesign Document (indd)
- Adobe Photoshop Document (psd)
- Advanced Audio Coding (aac)
- ALZ (alz)
- Android Binary XML (xml)
- Android Compiled Resources (arsc)
- ANI (ani)
- Animated Portable Network Graphics (apng)
- Apache Arrow Columnar (arrow)
- Apple Disk Image (dmg)
- Apple Icon Image (icns)
- Apple iTunes Audio (m4a)
- Apple iTunes Audiobook (m4b)
- Apple iTunes Protected Audio (m4p)
- Apple iTunes Video (m4v)
- Apple QuickTime (mov)
- Arbitrary Binary Data (bin)
- Archived by Robert Jung (arj)
- Au (au)
- Audio Codec 3 (ac3)
- Audio Interchange File Format (aiff)
- Audio Video Interleave (avi)
- AV1 Image File Format (avif)
- AV1 Image File Format Sequence (avifs)
- Better Portable Graphics (bpg)
- Blender (blend)
- bzip2 (bz2)
- Cabinet (cab)
- Canon Raw 2 (cr2)
- Canon Raw 3 (cr3)
- Cineon (cin)
- Compound File Binary (cfb)
- cpio (cpio)
- CUR (cur)
- Dalvik Executable (dex)
- Debian Binary Package (deb)
- Digital Imaging and Communications in Medicine (dcm)
- Digital Picture Exchange (dpx)
- Embedded OpenType (eot)
- Executable and Linkable Format (elf)
- Experimental Computing Facility (xcf)
- Extensible Archive (xar)
- FastTracker 2 Extended Module (xm)
- Flash Video (flv)
- Flexible Image Transport System (fits)
- Free Lossless Audio Codec (flac)
- Free Lossless Image Format (flif)
- Fujifilm Raw (raf)
- Game Boy Advance ROM (gba)
- Game Boy Color ROM (gbc)
- Game Boy ROM (gb)
- GL Transmission Format Binary (glb)
- Google Chrome Extension (crx)
- Graphics Interchange Format (gif)
- gzip (gz)
- High Efficiency Image Coding (heic)
- High Efficiency Image Coding Sequence (heics)
- High Efficiency Image File Format (heif)
- High Efficiency Image File Format Sequence (heifs)
- ICO (ico)
- Impulse Tracker Module (it)
- ISO 9660 (iso)
- Java Class (class)
- Java KeyStore (jks)
- Joint Photographic Experts Group (jpg)
- JPEG 2000 Part 1 (jp2)
- JPEG 2000 Part 1 (jpx)
- JPEG 2000 Part 3 (mj2)
- JPEG 2000 Part 6 (jpm)
- JPEG Extended Range (jxr)
- JPEG XL (jxl)
- Khronos Texture (ktx)
- Khronos Texture 2 (ktx2)
- Lempel–Ziv Finite State Entropy (lzfse)
- LHA (lzh)
- Long Range ZIP (lrz)
- LZ4 (lz4)
- lzip (lz)
- lzop (lzo)
- macOS Alias (alias)
- Material Exchange Format (mxf)
- Matroska Video (mkv)
- Microsoft Compiled HTML Help (chm)
- Microsoft DirectDraw Surface (dds)
- Microsoft Virtual Hard Disk (vhd)
- Microsoft Virtual Hard Disk 2 (vhdx)
- Mobipocket (mobi)
- Monkey’s Audio (ape)
- MPEG-1 Video (mpg)
- MPEG-4 Part 14 Video (mp4)
- MPEG-1/2 Audio Layer III (mp3)
- Musepack (mpc)
- Musical Instrument Digital Interface (mid)
- Nikon Electronic File (nef)
- Nintendo 64 ROM (z64)
- Nintendo DS ROM (nds)
- Nintendo Entertainment System ROM (nes)
- Ogg FLAC (oga)
- Ogg Media (ogm)
- Ogg Multiplexed Media (ogx)
- Ogg Opus (opus)
- Ogg Speex (spx)
- Ogg Theora (ogv)
- Ogg Vorbis (ogg)
- Olympus Raw Format (orf)
- OpenEXR (exr)
- OpenType (otf)
- Optimized Dalvik Executable (dey)
- Panasonic Raw (rw2)
- PCAP Dump (pcap)
- PCAP Next Generation Dump (pcapng)
- Portable Document Format (pdf)
- Portable Network Graphics (png)
- Qualcomm PureVoice (qcp)
- Radiance HDR (hdr)
- Red Hat Package Manager (rpm)
- Roshal Archive (rar)
- ScreamTracker 3 Module (s3m)
- SeqBox (sbx)
- 7-Zip (7z)
- Shapefile (shp)
- SketchUp (skp)
- Small Web Format (swf)
- Snappy (sz)
- Sony DSD Stream File (dsf)
- SQLite 3 (sqlite)
- Tag Image File Format (tiff)
- Tape Archive (tar)
- 3rd Generation Partnership Project (3gp)
- 3rd Generation Partnership Project 2 (3g2)
- TrueType (ttf)
- UNIX archiver (ar)
- UNIX compress (Z)
- VirtualBox Virtual Disk Image (vdi)
- WavPack (wv)
- Waveform Audio (wav)
- WebAssembly Binary (wasm)
- Web Open Font Format (woff)
- Web Open Font Format 2 (woff2)
- WebP (webp)
- Windows Bitmap (bmp)
- Windows Executable (exe)
- Windows Media Video (wmv)
- Windows Metafile (wmf)
- Windows Shortcut (lnk)
- XZ (xz)
- ZIP (zip)
- zoo (zoo)
- Zstandard (zst)

## License

This project is licensed under either of [Apache License, Version 2.0](LICENSE-APACHE) or [MIT license](LICENSE-MIT) at your option.
