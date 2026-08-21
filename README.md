# Hi there 👋

I work across **computer architecture, systems, HW/SW co-design, and verification methodology**.

I enjoy building things at the boundary between **architecture specifications, executable models, RTL, firmware, and system software** — especially when the problem calls for understanding the whole system rather than just one layer.

**Rust is my language of choice.**

## Selected projects

### [terminus](https://github.com/shady831213/terminus)
A RISC-V instruction-set and system simulator written in Rust.

- RV32/RV64 with I + M/A/F/D/C and M/S/U privilege modes
- Sv32 / Sv39 / Sv48 virtual memory, page-table walking, PMP and TLBs
- SMP Linux boot
- PLIC / CLINT
- VirtIO disk, network, console and input devices
- HDL co-simulation support

### [etha_model](https://github.com/shady831213/etha_model)
A Rust-based functional model for exploring **accelerator architecture and HW/SW interfaces**.

- RX/TX queue and DMA-descriptor architecture
- packet parsing, filtering, dispatch and arbitration pipelines
- software-visible register/interrupt interfaces
- Rust proc-macro DSLs that generate C register/descriptor headers
- IPsec/crypto acceleration and optional ROHC
- Chrome Trace based model observability and analysis

### [jarvisuk](https://github.com/shady831213/jarvisuk)
Reusable **SystemVerilog/UVM verification methodology infrastructure** for recurring SoC-level problems.

- memory allocation and backing models, including VA↔PA abstraction and memory attributes
- pin/MSI/software/shared interrupt infrastructure and vector redirection
- reusable register-region composition across reg blocks, sequencers and adapters
- clock/reset groups for multiple sources, frequencies, global/partial reset and sync/async reset
- thread-safe utility abstractions intended to be reused across verification environments

### [vfw_rs](https://github.com/shady831213/vfw_rs) · [mailbox_rs](https://github.com/shady831213/mailbox_rs) · [vhost](https://github.com/shady831213/vhost)
A Rust-based **host/target verification stack** for firmware-driven IC verification and HW/SW co-simulation.

- `vfw_rs`: `no_std` firmware runtime with multicore task execution, platform/HAL support, traps, runtime services and target-side mailbox integration
- `mailbox_rs`: C-compatible bounded request/response queues and extensible RPC, with `no_std` target-side and `std` host-side implementations
- `vhost`: host/simulator integration through memory backends, SystemVerilog DPI/UVM, optional Python callbacks and host services

The public repositories provide reusable infrastructure that can be extended with project-specific integrations in real verification environments.

### [terminus_cosim](https://github.com/shady831213/terminus_cosim)
A co-simulation environment connecting **RISC-V ISA models, RTL CPU cores, firmware, and the host verification environment**.

## Modeling & verification ecosystem

Several of these projects are reusable pieces around the same broader idea:

```text
architecture / HW-SW contracts
          │
          ├── terminus          executable CPU/system model
          ├── etha_model        accelerator architecture model
          │
          ├── terminus_vault    ISA/CSR definition and code generation
          ├── spaceport         memory/device/interrupt modeling substrate
          │
          ├── vfw_rs            target-side firmware verification runtime
          │       ↕
          ├── mailbox_rs        host/target protocol and RPC layer
          │       ↕
          ├── vhost             host/simulator integration
          │
          ├── terminus_cosim    ISA ↔ RTL co-simulation
          └── jarvisuk          reusable UVM verification methodology
```

I am interested in making architecture models, hardware/software interfaces, and verification infrastructure **composable rather than isolated artifacts**.

## Earlier project

### [algorithms](https://github.com/shady831213/algorithms)
An earlier CLRS study project in Go covering heaps, balanced trees, graph algorithms, shortest paths, flows, dynamic programming, greedy algorithms and sorting. It has received **800+ GitHub stars**.

## Public talk

- [Rust For IC design & Verification: vfw, vhost, terminus](https://www.bilibili.com/video/BV1qPe3ezE94/)

## Things I like thinking about

- Computer architecture and executable architecture models
- Hardware/software co-design and accelerator architecture
- Verification methodology and simulation infrastructure
- PCIe, IOMMU, virtualization and heterogeneous systems
- GPU system architecture
- Formal methods
- Systems research
- Rust for low-level systems and hardware tooling

I am particularly interested in problems where **architecture, verification, operating systems, and hardware meet**.

## Elsewhere

[LinkedIn](https://www.linkedin.com/in/%E6%97%B8-%E6%9D%8E-727095120)

> Still building things just for fun. :)
