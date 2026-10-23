<pre>
Rompass Labs
============
The open-source development space of Rompass. Focused on low-level system 
design, bare-metal embedded firmware, and micro-architecture exploitation.

Core Subsystems
---------------
* openc6-bios: An open-source RISC-V firmware platform for ESP32-C6 (8MB Flash).
  Implements a strict BIOS/Payload architecture with a custom system call 
  interface (ABI) and independent LP-Core coprocessor management.

Quick Start
-----------
* Report a bug: Open an Issue in the respective repository tracker.
* Get the latest source: <a href="https://github.com/Rompass/openc6-bios">Git clone https://github.com/Rompass/openc6-bios.git</a>
* Join the ecosystem: Review open feature requests and submit a clean PR.

Who Are You?
============
Find your role below:

* Payload Developer - Building bare-metal software on top of OpenC6 BIOS
* Subsystem Contributor - Hacking the core bootloader or filesystem layers
* Hardware Enthusiast - Testing custom RISC-V payloads on ESP32-C6 boards

For Specific Users
==================

Payload Developer
-----------------
Welcome to the ecosystem. To interface with the host platform:
* System Calls: Reference 'openc6_abi.h' inside your payload project.
* Execution Flow: Control is transferred via a direct jump with the 
  jump-table pointer passed through the 'a0' register.
* Constraints: Payload binaries must be fully static and position-independent 
  (-static -fPIE) to avoid structural relocation overhead.

Subsystem Contributor
---------------------
Help optimize and extend the core framework:
* Bare-metal C: Zero external dependencies. Avoid heavy runtime allocations.
* Memory Mapping: Keep the SRAM footprint strictly optimized. Every kilobyte 
saved increases target payload capacity.
  
Communication and Logs
======================
* GitHub Profile: <a href="https://github.com/Rompass/">https://github.com/Rompass/</a>
* Project Tracking: Review pinned repositories for active milestones and RFCs.
* Email: rompass@duck.com
</pre>
