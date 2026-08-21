# Hi there 👋

I work across **computer architecture, systems, and verification methodology**.

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

### [terminus_cosim](https://github.com/shady831213/terminus_cosim)
A co-simulation environment connecting **RISC-V ISA models, RTL CPU cores, firmware, and the host verification environment**.

### [vfw_rs](https://github.com/shady831213/vfw_rs) · [vhost](https://github.com/shady831213/vhost) · [mailbox_rs](https://github.com/shady831213/mailbox_rs)
Rust-based infrastructure for firmware-driven verification and HW/SW co-simulation, including multicore test execution, host/target communication, memory models, SystemVerilog DPI/UVM integration, and Python callbacks.

## Modeling & verification ecosystem

Several of these projects are reusable pieces around the same broader idea:

```text
architecture / HW-SW interface
          │
          ├── terminus       executable CPU/system model
          ├── etha_model     accelerator architecture exploration
          │
          ├── terminus_vault ISA/CSR definition and code-generation tooling
          ├── spaceport      memory/device/interrupt substrate
          │
          ├── terminus_cosim ISA ↔ RTL co-simulation
          ├── vfw / vhost    firmware + host verification infrastructure
          └── jarvisuk       reusable UVM verification methodology
```

I am interested in making architecture models, hardware/software interfaces, and verification infrastructure **composable rather than isolated artifacts**.

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
