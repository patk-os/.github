


____       _  _____ _  __      ___  ____  
 |  _ \     / \|_   _| |/ /     / _ \/ ___| 
 | |_) |   / _ \ | | | ' /_____| | | \___ \ 
 |  __/   / ___ \| | | . \_____| |_| |___) |
 |_|     /_/   \_\_| |_|\_\     \___/|____/ 
                                             
  >> Ring 0 is not a nightclub. Get the drivers out. <<

Welcome to the PanicAtTheKernel Organization

The era of monolithic complexity has reached its breaking point. Linux and Windows pack tens of millions of lines of third-party driver code into Ring 0, where a single memory safety violation brings down entire infrastructures.

PATK-OS is an uncompromising, crash-proof, microkernel-based operating system designed natively for modern 64-bit architectures.

Lineage & Foundation
PATK-OS is directly forged from the proven architectural DNA of the MINIX 3 microkernel and NetBSD userland heritage. We are standing on the shoulders of Andrew S. Tanenbaum’s pure microkernel vision—stripping decades of historical 32-bit technical debt and resurrecting the codebase into a high-performance, modern x86_64 reality. Tanenbaum was right: microkernels are the future. We are just 30 years late to finish the job for modern bare-metal.

Key Pillars of the Architecture
🛡️ Absolute Kernel Isolation: The Ring 0 core strictly executes scheduling, memory management (paging), and register-optimized IPC. Nothing else.
💀 Fault Containment (Ring 3): File systems, network stacks, and hardware drivers live entirely in userspace. Drivers can crash and be restarted in microseconds without taking down the kernel.
⚡ Pure x86_64: Stripped of 16-bit real-mode legacy, antique ISA routing, and 32-bit bloat. Built directly for modern multi-core silicon.
📜 Permissive & Open: No GPL infection. Built with respect for true open-source freedom under the BSD 3-Clause License.

Core Repositories
Repository      Description                                           Status
patk-kernel     Pure C & ASM x86_64 microkernel core (Ring 0)         Active Surgery
patk-os         Complete OS distribution tree, build harnesses, & tools Architecture

The Call for Low-Level Hackers
We are building this because we are exhausted by corporate-driven bloatware disguised as modern operating systems.

If you write C, C++, and x86_64 Assembly, and you care about determinism, bare-metal efficiency, and true microkernel isolation:

$ git clone https://github.com/panicatthekernel/patk-kernel.git
$ cd patk-kernel && make

Monoliths panic. Microkernels prevail.
