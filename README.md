#  WOR | Digital Privacy & Metadata Forensic Suite

![Project Status](https://img.shields.io/badge/Status-In--Development-yellow?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Security](https://img.shields.io/badge/Security-Metadata%20Sanitization-blue?style=flat-square)

**WOR** is a professional-grade cybersecurity utility designed to audit image forensics and sanitize tracking metadata. The platform addresses the critical vulnerability of hidden EXIF data, providing users with the tools to extract, analyze, and permanently erase geographical and device-specific traces.

---

##  Core Functionalities

### 1. Forensic Metadata Extraction
The system performs a deep binary scan of image headers to retrieve embedded metadata, including:
* **Geospatial Data:** GPS Latitude, Longitude, and Altitude.
* **Device Specifications:** Manufacturer, Model, and Software Version.
* **Temporal Markers:** Precise timestamps and digitizing dates.

### 2. Privacy Sanitization (The Stripper)
Using an advanced **Canvas Reconstruction** technique, WOR destroys the original EXIF/IPTC/XMP headers. By redrawing the image at the pixel level, the system ensures that the output file is mathematically devoid of any previous metadata while maintaining visual integrity.

---

##  Practical Application: A Security Walkthrough

To demonstrate the inherent risks of unmanaged metadata, WOR follows a three-step forensic workflow:

1. **Identification:** User uploads a raw image; the engine identifies hidden GPS coordinates.
2. **Visualization:** The system maps the raw data to a physical location, highlighting the precision of the potential leak.
3. **Mitigation:** The "Privacy Stripper" module processes the image, generating a sanitized version ready for secure distribution.

---

##  Technical Architecture

* **Environment:** Client-Side Execution (Browser-based).
* **Processing Engine:** HTML5 Canvas API & EXIF.js Logic.
* **Data Privacy:** Zero Server-Side interaction; all processing is volatile and occurs within the local memory.
* **Optimization:** Designed for high-performance rendering on modern hardware.

---

##  Project Roadmap

- [x] High-fidelity UI/UX Implementation.
- [x] GPS Forensic Mapping Engine.
- [x] Metadata Sanitization Module.
- [ ] Support for multi-format processing (PNG/WebP).
- [ ] Source Code Obfuscation for enhanced integrity.

---

## Lead Developer
**Ahmed** *Systems Architect & Cybersecurity Specialist*

---
> **Disclaimer:** This tool is intended for educational and security awareness purposes. Users are responsible for ensuring compliance with local privacy laws and regulations.
