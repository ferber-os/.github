# Ferber

**Zero ambient authority. Programs earn every resource they touch.**

Ferber is an open-source operating system project built around explicit resource authority, strong isolation, and a capability-based microkernel written in Rust.

The project targets RISC-V64 and x86-64, with a focus on keeping privileged mechanisms small and moving operating-system functionality into userspace.

## The ecosystem

Ferber is more than its kernel. The project encompasses several components as development progresses:

- **Ferber** — The capability-based microkernel, responsible for isolation, scheduling, memory management, IPC, and resource authority.
- **Ferrum** — The userspace environment, including initialization, system services, and eventually an interactive shell.
- **Libraries and SDKs** — Interfaces for building native applications against Ferber's system ABI.
- **Compatibility and ports** — Work toward supporting existing software, including a future musl libc port.
- **Developer tooling** — Build tools, debugging utilities, testing infrastructure, and supporting documentation.

These components are at different stages of development. Some are implemented, others are planned.

## Repositories

### [ferber](https://github.com/ferber-os/ferber)

The main development repository.

Contains the microkernel, boot infrastructure, shared ABI definitions, Ferrum components, build tooling, and cross-architecture verification.

Additional repositories will be created as components develop independent maintenance and release requirements.

## Development status

Ferber is experimental and under active development. It is not currently a production operating system.

Development priorities include userspace process creation, capability delegation, resource accounting, and the mechanisms needed for independently launched services.

The project is tested through automated host and QEMU verification on both target architectures, with additional physical x86-64 hardware testing.

## Contributing

Contributions, bug reports, technical reviews, and discussions are welcome.

See the main repository's [contribution guidelines](https://github.com/ferber-os/ferber/blob/main/CONTRIBUTING.md) for development and submission information.

## Links

**Project source:** https://github.com/ferber-os/ferber

**Technical articles:** https://notvc.to

**Maintainer:** [notvcto](https://github.com/notvcto)
