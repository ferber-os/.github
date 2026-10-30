<p align="center">
  <img src="https://raw.githubusercontent.com/ferber-os/ferber/main/docs/assets/ferber.png" width="180" alt="Ferber logo">
</p>

# Ferber

Capability-based systems in Rust. Programs receive authority explicitly. Handles,
mappings and the memory behind them have separate lifetimes. The kernel has to
account for all three.

[Ferber](https://github.com/ferber-os/ferber) is a microkernel targeting RISC-V64
and x86-64. It runs independently compiled userspace programs, provides
capability-aware IPC and manages sparse physical memory. Ferrum is its userspace
implementation, starting with a resident `init`. Service launch and an interactive
shell are still ahead.

Both architectures are tested in QEMU. Physical x86-64 validation runs on a
32 GiB workstation. Physical RISC-V testing would be useful; no such hardware
is currently available here.

The [roadmap](https://github.com/ferber-os/ferber/blob/main/ROADMAP.md) tracks what
works and what remains. For a first contribution, start with the
[contribution guide](https://github.com/ferber-os/ferber/blob/main/CONTRIBUTING.md).
Documentation, testing and tooling are useful work. Your first patch does not
need to touch the kernel.

[Technical writeups](https://notvc.to/blog) cover the implementation and its
failure cases.
