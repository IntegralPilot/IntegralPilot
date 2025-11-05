# 👋 Hey there! I'm Michael (aka IntegralPilot)

I'm passionate about **low-level systems**, **security research**, and **compiler design**.

🎯 **TL;DR** - I build operating systems, compilers, and CPUs from scratch. I've discovered **high-severity security vulnerabilities** in Apple macOS ([**CVE-2025-43361**](https://www.cve.org/CVERecord?id=CVE-2025-43361)), wrote a **compiler** to bring Rust to the JVM, contributed code that powers **Wikipedia's backend**, and shipped production apps with **Flutter and TypeScript**.

---

### 🛡️ Security Research & Disclosures

I contribute to security through responsible disclosure.

| CVE ID      | Product      | Summary                                | Status                                                 |
| ----------- | ------------ | -------------------------------------- | ------------------------------------------------------ |
| **CVE-2025-43361** | Apple macOS, iOS, tvOS, visionOS, watchOS  | A malicious sandboxed app may be able to read kernel memory through an issue in the Audio subsystem. [Vendor advisory](https://support.apple.com/en-us/125108), [CVE.org](https://www.cve.org/CVERecord?id=CVE-2025-43361)| Assigned **CVSS 7.8 (HIGH)**, patched and published.  |

> *Several other vulnerabilities are currently in the process of coordinated disclosure. They will be listed here once publicly announced.*
---

### 👨‍💻 About Me

- 🇦🇺 High school sophmore (Year 10) based in Australia  
- 🧠 Deep interest in systems programming, hardware design, and applied security  
- 🧬 Exploring computational neuroscience and bioinformatics  
- ⚡ I love building things that are fast, safe, and deeply understood

---

### 🚀 Featured Projects

Here are a few projects I'm especially proud of - spanning operating systems, compiler internals, hardware, and computational science.

| Project                                                                            | Description                                                                                                                                     | Key Technologies                            |
| ---------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| ☕ **[rustc_codegen_jvm](https://github.com/IntegralPilot/rustc_codegen_jvm)**     | Custom Rust compiler backend targeting JVM bytecode. Compile Rust to a `.jar` to run on any JVM.<br>- **Supports**: Control flow, ADTs, generics, closures, traits, dynamic dispatch, etc.<br>- **Tooling**: Includes a custom Python-based build/test system and seamless Java interop.                                                                  | `Rust`, `Compilers`, `JVM`  |
| 🦀 **[WasmOS](https://github.com/IntegralPilot/wasm_os)**                           | Experimental x86_64 unikernel OS in Rust, designed from scratch to run WebAssembly-based userspace apps.<br>- **Supports**: Rust, C, C++ and AssemblyScript userspace programs compiled to WASM.<br>- **Features:** Custom libc/libstd++ and ABI design, and VFS/inode system.                                                | `Rust`, `WASM`, `x86_64`                    |
| ⚡ **[GammaCPU](https://github.com/IntegralPilot/GammaCPU)**                       | A 32-bit, stack-based CPU in VHDL executing a subset of the WASM instruction set, including a custom stack and ALU component, and integration and unit testing system. (Built with @aellul27.)                                      | `VHDL`, `WASM`, `Hardware`                  |
| 🧠 **[DynamicSNN](https://github.com/IntegralPilot/DynamicSNN)**                   | C++ simulator for biologically plausible learning in Spiking Neural Networks, modeling synergy in plasticity mechanisms. Features modern C++17 design principles including smart pointers and CMake, and easy to use Python wrapper API.                      | `C++`, `Neuroscience`, `Python`             |

---

🌍 <strong>Open Source Contributions</strong>

I actively contribute to open source, including the Wikimedia Foundation’s MediaWiki platform - my code is live on Wikipedia.

| Project            | Contribution Summary                                                                                       | Links                                                                                                   |
| ------------------ | ---------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| **MediaWiki – Nuke** *(merged & deployed)* | ✨ Filtering by min/max page size in `Special:Nuke`, with UI, backend logic, and validation. <br>🔍 Introduced non-fatal validation messages. | [Change 1116491](https://gerrit.wikimedia.org/r/c/mediawiki/extensions/Nuke/+/1116491) <br>[T378488](https://phabricator.wikimedia.org/T378488) |
| **MediaWiki – Nuke** *(merged & deployed)* | 🔓 Allowed non-admins to list pages in `Special:Nuke`, improving usability for patrollers. <br>🛑 Permission-aware UI and i18n. | [Change 1116493](https://gerrit.wikimedia.org/r/c/mediawiki/extensions/Nuke/+/1116493) <br>[T376378](https://phabricator.wikimedia.org/T376378) |
| **MediaWiki – AbuseFilter** *(under review)* | 🕵️ Added support for *suppressing* filters containing PII. <br>👥 UI/API access restricted to oversighters. | [Change 1115319](https://gerrit.wikimedia.org/r/c/mediawiki/extensions/AbuseFilter/+/1115319) <br>[T290324](https://phabricator.wikimedia.org/T290324) |

---
📱 <strong>Apps</strong>

Outside of systems work, I build applications that solve real-world problems - especially in education, accessibility, and healthcare.

| App Name          | Description                                                                                                                                                   | Tech Stack                                      | Links                                                                                                                                       |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| 🎵 **MelodyRex**  | Built a music practice companion for students/teachers, built in 8th grade. Still in use at my school.                                                                | `TypeScript`, `Vite`, `Firebase`, `Swift`       | [Website](https://melodyrex.pages.dev/get), [App Store](https://apps.apple.com/au/app/melodyrex-music-practice-tool/id6468330380)         |
| 🧬 **ClarityScreen** | Designed a concept app with working backend for clear and accessible display of Alzheimer’s genetic test results.                                                                        | `Flutter`, `Dart`, `Firebase`                   | [Website](https://clarityscreen.pages.dev)                                                                                                 |
| 👁️ **4Sight**     | Created an AI-powered assistant for low vision. Describes surroundings, reads signs/maps, and answers camera-based queries using LLMs and custom CNNs.                  | `Flutter`, `Dart`, `Azure`, `Google Gemini`     | [Website](https://4sight.pages.dev), [App Store](https://apps.apple.com/us/app/4sight-ai-for-real-life/id6505015586)                      |

---

### 💻 <strong>Languages</strong>

- **Expert:** Rust, C++, Python, Git, ARM Assembly (arm64, arm64e w/ PAC)
- **Proficient:** VHDL, C, x86_64 Assembly, Java, Kotlin, TypeScript, Flutter
- **Learning:** Lean (for mathematical proofs and formal verification)

### 🔧 <strong>Tools</strong>

- **Systems & Low-Level:** QEMU, LLDB, LLVM, Vivado, GHDL
- **Security:** Ghidra, Frida, Jackalope (fuzzer), TinyInst

---

### 🔭 Currently Working On

- Expanding `rustc_codegen_jvm` to support more of the Rust language.
- FPGA accelerator for [cryogenic electron microscopy](https://en.wikipedia.org/wiki/Cryogenic_electron_microscopy).
- Developing a Rust-based platform for XNU kext fuzzing in userspace.
- Learning Lean for formal verification.

---

### 📫 Get in Touch

- **Email**: `linux479 [at] duck [dot] com`
- **Discord**: `dna_codon`
- **Reddit**: `u/IntegralPilot`
