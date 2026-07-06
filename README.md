# Hey there! I'm Michael (aka IntegralPilot)

I'm passionate about **low-level systems**, **security research**, and **compiler design**.

I focus on identifying vulnerabilities in platforms like iOS and macOS, building compiler tooling, and contributing to core open-source infrastructure. My work ranges from kernel-level development to cross-platform application design.

## Security Research & Disclosures

I participate in vulnerability research and responsible disclosure. Below are some of my recent findings:

| CVE ID | Component | Vulnerability Detail | References | CVSS 
| :--- | :--- | :--- | :--- | :--- |
| **CVE-2025-43361** | **Apple Audio Subsystem** | **Kernel Memory Disclosure.** Out-of-bounds read in a kernel extension accessible from sandboxed applications. | [Vendor (iOS)](https://support.apple.com/en-us/125108)<br>[CVE.org](https://www.cve.org/CVERecord?id=CVE-2025-43361) | 7.8 (HIGH)
| **CVE-2025-43539** | **AppleJPEG**<br>JPEG XL (JXL) | **Memory Corruption** in `AppleJPEG` during JPEG XL parsing. Zero-click remote vector. | [Vendor (iOS)](https://support.apple.com/en-us/125884)<br>[CVE.org](https://www.cve.org/CVERecord?id=CVE-2025-43539) | 8.8 (HIGH)
| **CVE-2025-43482** | **Apple CoreAudio**<br>`coreaudiod` | **Denial of Service.** Improper input validation in the system audio daemon. Co-credited with Jex Amro. | [Vendor (macOS)](https://support.apple.com/en-us/125886)<br>[CVE.org](https://www.cve.org/CVERecord?id=CVE-2025-43482) | 5.5 (MEDIUM)

## About Me

- High school student (Year 11) based in Australia  
- Deep interest in systems programming, hardware design, and applied security  
- Exploring computational neuroscience and bioinformatics  
- Focused on building fast, safe, and deeply understood systems

## Open Source Contributions

I actively contribute to upstream open-source projects, focusing on kernels, runtimes, and core web infrastructure.

### Linux Kernel (Asahi Linux)

| Component | Contribution Summary | Links |
| :--- | :--- | :--- |
| **Mac SMC power drivers** | Refactored and upstreamed the `macsmc-power` driver, enabling battery telemetry, AC adapter monitoring, and charge control on Apple Silicon. | [v7 Patchset (shipped in v7.1)](https://lore.kernel.org/asahi/20260217-b4-macsmc-power-v7-0-4a4d63664362@gmail.com/) |
| **Mac DockChannel HID drivers** | Co-authored the `apple-dockchannel` mailbox driver and `apple-hid` transport driver to support built-in keyboards on M2 and M3 MacBooks. | [v1 Patchset (WIP)](https://lore.kernel.org/asahi/20260630-apple-mtp-keyboard-final-v1-0-506d936a1707@gmail.com/) |

### OpenJDK

I contribute to the **HotSpot C2 compiler** to study optimisation techniques in managed runtimes. 

My most impactful change was probably the **128-bit Multiplication optimisation (x86_64)**, which mproved performance of 128-bit multiplication operations by approximately 1.85x on x86 platforms.

The PR is here: [OpenJDK PR #30174](https://github.com/openjdk/jdk/pull/30174). *Note: The PR is marked as "Closed" on GitHub due to OpenJDK's Skara bot workflow, but the change was accepted and integrated into mainline, after really useful feedback that I am super grateful for.*

### MediaWiki

| Project | Contribution Summary | Links |
| :--- | :--- | :--- |
| **Nuke Extension** | Implemented min/max page size filtering in `Special:Nuke` with UI validation and non-fatal warning messages. | [Change 1116491](https://gerrit.wikimedia.org/r/c/mediawiki/extensions/Nuke/+/1116491) |
| **Nuke Extension** | Enabled non-administrators (e.g., patrollers) to list pages, introducing permission-aware UI and localizations. | [Change 1116493](https://gerrit.wikimedia.org/r/c/mediawiki/extensions/Nuke/+/1116493) |
| **AbuseFilter** | Added support for suppressing filters containing PII, restricting access to oversighters. | [Change 1115319](https://gerrit.wikimedia.org/r/c/mediawiki/extensions/AbuseFilter/+/1115319) |


## Featured Personal Projects

### Software
Here are some of my various hobby/experimenting projects on GitHub. They projects span operating systems, compiler internals, hardware, and computational science.

| Project | Description | Key Technologies |
| :--- | :--- | :--- |
| **[rustc_codegen_jvm](https://github.com/IntegralPilot/rustc_codegen_jvm)** | Custom Rust compiler backend targeting JVM bytecode. Compiles Rust to runnable `.jar` files.<br>- **Supports**: Control flow, ADTs, generics, closures, traits, and dynamic dispatch.<br>- **Tooling**: Custom Python-based build/test system with Java interop. | `Rust`, `Compilers`, `JVM` |
| **[WasmOS](https://github.com/IntegralPilot/wasm_os)** | Experimental x86_64 unikernel OS written in Rust, designed to run WebAssembly-based userspace apps.<br>- **Features**: Custom libc/libstd++, ABI design, and a virtual file system (VFS). | `Rust`, `WASM`, `x86_64` |
| **[GammaCPU](https://github.com/IntegralPilot/GammaCPU)** | A 32-bit, stack-based CPU in VHDL executing a subset of the WASM instruction set. Includes a custom ALU and integration testing suite. Developed with aellul27. | `VHDL`, `WASM`, `Hardware` |
| **[DynamicSNN](https://github.com/IntegralPilot/DynamicSNN)** | C++ simulator for learning in Spiking Neural Networks, modeling synergy in plasticity mechanisms. Features a modern C++17 design with a Python wrapper API. | `C++`, `Neuroscience`, `Python` |

### Hardware

I also made a hardware project, CryoFlow, which was a FPGA to accelerate [Cryo-EM](https://en.wikipedia.org/wiki/Cryo-electron_microscopy) data processing. Cryo-EM is important for researching diseases like Alzheimer's but currently bottlenecked by GPUs which waste excess energy and water for cooling, and are expensive to obtain nowadays with the LLM boom. 

I implemented a custom FPGA pipeline using a mix of VHDL and HLS C++, and took some inspiration from Apple Unified Memory and Systolic Arrays in Google TPUs. I achieved an ~8.6x improvement in performance per Watt compared to the RTX 3080. The project involved a custom system architecture I designed, including a WebSerial (over USB-UART) dashboard to enable easy use and custom Rust-based firmware running on the Arm cores.

I presented it at [ISEF 2026](https://en.wikipedia.org/wiki/International_Science_and_Engineering_Fair) and was very grateful to come 2nd in my category of Embedded Systems and recieved special awards from the International Council on Systems Engineering and Society for Science Alumni Association.

You can see my poster [here.](https://drive.google.com/file/d/1WxJn78v57I-nhOd5zNDbrQN8s-FZlOpy/view)

## Applications

I also design applications aimed at education, accessibility, and assistive healthcare.

| App Name | Description | Tech Stack | Links |
| :--- | :--- | :--- | :--- |
| **MelodyRex** | A music practice companion for students and teachers. Built in 8th grade and currently utilized in educational programs. | `TypeScript`, `Vite`, `Firebase`, `Swift` | [Website](https://melodyrex.pages.dev/get) \| [App Store](https://apps.apple.com/au/app/melodyrex-music-practice-tool/id6468330380) |
| **ClarityScreen** | Concept application and backend for clear, accessible rendering of Alzheimer’s genetic test results. | `Flutter`, `Dart`, `Firebase` | [Website](https://clarityscreen.pages.dev) |
| **4Sight** | AI-powered assistant for low-vision users. Describes environments, parses text/maps, and handles visual queries. | `Flutter`, `Dart`, `Azure`, `Gemini` | [Website](https://4sight.pages.dev) \| [App Store](https://apps.apple.com/us/app/4sight-ai-for-real-life/id6505015586) |

## Skills

### Languages

* **Advanced:** Rust, C++, Python, ARM Assembly (including ARM64e with PAC)
* **Proficient:** VHDL, C, x86_64 Assembly, Java, Kotlin, TypeScript, Dart (Flutter)
* **Learning:** Lean (for formal verification and mathematical proofs)

### Tooling & Environments

* **Systems/Low-Level:** QEMU, LLDB, LLVM, Vivado, GHDL
* **Security & Analysis:** Ghidra, Frida, Jackalope, TinyInst

---

## Get in Touch

- **Email**: `linux479 [at] duck [dot] com`
- **Discord**: `dna_codon`
- **Reddit**: `u/IntegralPilot`
- **Twitter/X**: `@IntegralPilot`
- **Bluesky**: `@integralpilot.bsky.social`
