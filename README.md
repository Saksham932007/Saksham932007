# Saksham Kapoor

### Backend & Systems Engineer | Rust · C · C++ · Node.js · Distributed Systems

I build systems from the ground up — from operating system kernels and storage engines to distributed databases and high-performance backend infrastructure.

My interests lie in understanding what happens beneath applications: memory management, concurrency, storage, replication, networking, and the engineering trade-offs that shape reliable software.

- 🎓 **BCA (AI/ML)** at Chaudhary Charan Singh University (CCSU), graduating July 2027.
- 💻 Currently working as a **Software Developer Intern**, building production web products and backend systems.
- 🔬 Submitted research on observability overhead in Redis-compatible servers.
- 🌱 Interested in distributed systems, databases, operating systems, backend engineering and infrastructure.
- 🤝 Open to collaborating on systems programming, databases, infrastructure and open-source projects.

📍 Delhi, India  
📧 [sakshamkapoor810@gmail.com](mailto:sakshamkapoor810@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/sakshamkapoor-eng/) · [Portfolio](https://saksham932007.github.io/Saksham932007/) · [GitHub](https://github.com/Saksham932007)

---

## Featured Engineering Projects

I enjoy building software from first principles, particularly systems where correctness, performance and reliability matter.

### 1. StratumOS — Operating System Kernel & Bootloader

**C · x86 Assembly · Operating Systems · Memory Management**

An x86 operating system kernel and bootloader built from scratch, progressing from a 32-bit real-mode bootloader to a preemptive, paged, multi-processor system.

**Architecture and implementation**

- Custom bootloader with FAT16 disk execution.
- Copy-on-write fork and process execution.
- Preemptive multitasking and multi-processor bring-up.
- Four-CPU SMP bring-up.
- Network stack supporting ARP, IPv4, ICMP, UDP and TCP.
- Hardware and kernel/user memory protection.
- W^X, SMEP/SMAP and guard-page protections.

**Verification and testing**

- 633 kernel assertions and 12 QEMU boot scenarios in CI.
- Fuzzing with 4 LibFuzzer targets.
- 40,000 malformed syscalls tested.
- Fuzzing uncovered 6 bugs.
- Ported kernel sources to RISC-V 64, with 16 of 29 files built unmodified.

🔗 **[View StratumOS Repository](https://github.com/Saksham932007/StratumOS)**

---

### 2. KestrelCache — Persistent Key-Value Database with Raft Replication

**C# · .NET 9 · Distributed Systems · Storage Engines**

A persistent key-value database developed from scratch, combining storage-engine design, Redis-compatible networking and distributed replication.

**Architecture**

- Two storage engines:
  - Bitcask-style log-structured storage.
  - LSM-tree with WAL, SSTables and Bloom filters.
- Redis-protocol server compatible with an unmodified Redis client.
- Raft replication with snapshots.
- Joint-consensus membership changes.
- Crash recovery and persistent storage.

**Correctness and performance**

- 308 tests, including SIGKILL crash-consistency tests.
- Raft log verification under message loss.
- Group commit performance measured between 49K and 82K ops/s.
- Batched fsync improved per-key throughput by up to 392x.
- Bloom filter false-positive rate reduced from 0.8% to 0.7%.
- Measured GET throughput reaching 662K GET/s.

🔗 **[View KestrelCache Repository](https://github.com/Saksham932007/KestrelCache)**

---

### 3. RustRedis — Redis-Compatible Server & Observability Research

**Rust · Tokio · Redis Protocol · Benchmarking · Research**

A Redis-compatible server implemented in Rust using Tokio, accompanied by a reproducible research study investigating the performance overhead of observability instrumentation.

**Engineering**

- Approximately 3,500 lines of Rust.
- Redis-compatible server implementation.
- Eight interchangeable metrics collectors.
- Designed to isolate individual observability instrumentation costs.
- Benchmarking infrastructure for controlled performance experiments.

**Research**

- 29,520 benchmark runs.
- 14 Azure VMs.
- Workloads covering 100–3,000 clients.
- Three distinct workloads.
- Randomized interleaved trials and run-clustered confidence intervals.
- Investigated the impact of metric cardinality on throughput.

**Key finding**

A high-cardinality metric label cost 0.87 percentage points of throughput, approximately 1.66x the 0.52 percentage-point cost observed when replacing a global mutex with a 64-way sharded map.

📄 Research paper: *Cardinality Before Contention: Observability Overhead in a Rust/Tokio Redis-Compatible Server.*

Submitted to *Software: Practice and Experience* (October 2026). Preprint available; not yet peer-reviewed.

🔗 **[View RustRedis Repository](https://github.com/Saksham932007/RustRedis)**

---

## Professional Experience

### Software Developer Intern

**Software Consultancy | July 2026 – Present**

Working on production software products across multiple client projects.

- Delivering end-to-end features across frontend, backend and database layers.
- Designing database schemas, migrations, service layers and REST APIs.
- Integrating third-party APIs into customer-facing product workflows.
- Working across multiple codebases, adapting to different technology stacks and conventions.
- Collaborating with developers through code reviews and feature delivery.

**Technologies:** React, Next.js, Node.js, REST APIs, PostgreSQL, MongoDB and database migrations.

### Open Source Mentor — GirlScript Summer of Code

**July 2025 – February 2026**

- Mentored contributors working on DraftDeckAI, an AI-powered document creation platform.
- Helped contributors understand unfamiliar codebases and development workflows.
- Reviewed pull requests and provided feedback on implementation quality and project conventions.

### E-Cell, IIT Bombay

**Mentor and Campus Ambassador | 2025**

- Mentored student founders and helped evaluate startup ideas.
- Supported student participation in entrepreneurship programmes.
- Helped aspiring founders think through product feasibility and market opportunities.

---

## Research & Publications

### Cardinality Before Contention

*Observability Overhead in a Rust/Tokio Redis-Compatible Server*

An empirical investigation into the performance costs of observability instrumentation in Redis-compatible systems.

- 29,520 benchmark runs across 14 Azure VMs.
- Eight interchangeable metrics collectors.
- Controlled experiments with randomized trials.
- Analysis of metric cardinality and synchronization overhead.

**Status:** Preprint submitted to *Software: Practice and Experience*. Not yet peer-reviewed.

---

## Technical Skills

### Programming Languages

- Rust
- C
- C++
- C#
- Python
- JavaScript
- TypeScript
- Java

### Systems & Low-Level Engineering

- Operating Systems
- Kernel Development
- Memory Management
- Concurrency and Multithreading
- x86 Assembly
- Linux
- Networking and TCP/IP
- Process Management

### Backend & Distributed Systems

- Node.js
- NestJS
- React
- Next.js
- REST APIs
- Distributed Systems
- Raft Consensus
- Database Internals
- Redis Protocol
- PostgreSQL
- MongoDB
- Prisma ORM

### Storage & Infrastructure

- LSM Trees
- Write-Ahead Logging
- SSTables
- Bloom Filters
- Bitcask Storage
- Docker
- Git
- CI/CD
- Linux

### Testing & Research

- Unit and Integration Testing
- QEMU
- LibFuzzer
- Crash Consistency Testing
- Performance Benchmarking
- Statistical Analysis
- Observability

---

## Competitive Programming

I regularly practise algorithmic problem-solving and participate in programming contests.

- **LeetCode:** 158+ problems solved.
- **LeetCode Contest Rating:** 1570.
- **CodeChef:** Competitive programming participant.

Profiles:

- [LeetCode](https://leetcode.com/)
- [CodeChef](https://www.codechef.com/)

---

## Education

**Bachelor of Computer Applications (BCA) — AI/ML**

Chaudhary Charan Singh University (CCSU), Meerut  
September 2024 – July 2027 (Expected)

---

## Certifications

Some of my selected professional and technical certifications:

- Oracle Cloud Infrastructure 2025 Certified Generative AI Professional.
- Google AI Essentials.
- Google Data Analytics.
- Cisco Data Analytics Essentials.
- Microsoft 365.
- MIT — Accounting and Planning.

---

## Languages

- English — Native or bilingual proficiency.
- Korean — Professional working proficiency.
- Chinese — Limited working proficiency.

---

## What I'm Interested In

I'm particularly interested in engineering problems involving:

- Building databases and storage engines from scratch.
- Distributed systems and consensus algorithms.
- Operating systems and kernel development.
- High-performance backend infrastructure.
- Concurrency, networking and memory management.
- Observability and performance engineering.

I'm always interested in collaborating with engineers who enjoy understanding systems at a deeper level.

---

## Let's Connect

If you're working on something involving systems programming, distributed databases, backend infrastructure or open-source engineering, I'd love to connect.

- **LinkedIn:** https://www.linkedin.com/in/sakshamkapoor-eng/
- **Portfolio:** https://saksham932007.github.io/Saksham932007/
- **Email:** sakshamkapoor810@gmail.com

---

*Build from first principles. Measure before optimizing. Understand the layer below.*
