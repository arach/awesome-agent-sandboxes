# Awesome Agent Sandboxes [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> An exhaustive map of the agent execution layer: sandboxes, microVMs, code-execution APIs, cloud workspaces, agent hosting, and computer-use VMs — everything that runs AI agents safely. Curated by [AgentList.io](https://www.agentlist.io).

**419 entries across 8 sections.** Every entry links to its canonical source; GitHub-backed entries carry stars, license, and activity metadata. `📦 archived` means the repository is archived or the project is dead; `💤 dormant` means no pushes in over a year.

## Contents

- [Agent Sandboxes](#agent-sandboxes) (80)
- [MicroVMs & Hardware Isolation](#microvms--hardware-isolation) (68)
- [Code Execution APIs & Interpreters](#code-execution-apis--interpreters) (86)
- [Cloud Workspaces & Dev Environments](#cloud-workspaces--dev-environments) (48)
- [Agent Hosting & Deployment](#agent-hosting--deployment) (33)
- [Computer-Use VMs & Desktop Sandboxes](#computer-use-vms--desktop-sandboxes) (37)
- [Isolation Utilities & SDKs](#isolation-utilities--sdks) (57)
- [Dormant & Archived (Notable)](#dormant--archived-(notable)) (10)

## Agent Sandboxes

*Sandboxed runtimes purpose-built for agent code execution — containers, gVisor/Kata, and per-task isolation.*

- [Deno Sandboxes](https://deno.com) — Deno's hosted sandbox service for short-lived isolated code execution. *(★ 108.5k, MIT)*
- [Daytona](https://www.daytona.io) — Sandbox infrastructure for AI-generated code. The public repository says it is no longer maintained as of June 2026. *(★ 71.7k)*
- [OpenSandbox](https://open-sandbox.ai) — Alibaba sandbox runtime with pluggable Docker, gVisor, Kata, and Firecracker backends. *(★ 15.6k, Apache-2.0)*
- [E2B](https://e2b.dev) — Firecracker microVM cloud for running agent-generated code, with a code-interpreter SDK and desktop sandboxes. *(★ 14k, Apache-2.0)*
- [SandBase Sandbox](https://www.sandbase.ai/sandbox) — Hosted sandbox gateway that lets agents run commands and retrieve files through the E2B SDK.
- [microsandbox](https://microsandbox.dev) — Embeddable libkrun microVM SDK that boots OCI images and keeps secrets on the host. *(★ 8.5k, Apache-2.0)*
- [AIO Sandbox](https://sandbox.agent-infra.com) — All-in-one agent container image with a browser, shell, VS Code, Jupyter, and MCP. *(★ 6k, Apache-2.0)*
- [Kubernetes Agent Sandbox](https://agent-sandbox.sigs.k8s.io) — Kubernetes APIs for agent workloads with pluggable gVisor and Kata isolation. *(★ 4.1k, Apache-2.0)*
- [AgentENV](https://github.com/kvcache-ai/AgentENV) — Self-hosted Firecracker environment manager for agent sandboxes and templates. *(★ 3.6k, MIT)*
- [Beam](https://www.beam.cloud) — Open-source serverless runtime with gVisor or runc sandboxes, GPU checkpoint restore, and task queues. *(★ 1.8k, AGPL-3.0)*
- [Sandbox Agent](https://sandboxagent.dev) — HTTP API that runs Claude Code, Codex, OpenCode, and Amp inside a sandbox. *(★ 1.6k, Apache-2.0)*
- [Dormice](https://github.com/BitMiracle-AI/Dormice) — Self-hosted E2B-compatible sandbox server that keeps sandboxes resident on one machine. *(★ 1.3k, Apache-2.0)*
- [Cloudflare Sandboxes](https://developers.cloudflare.com/sandbox/) — Container sandboxes on Cloudflare with a shell, filesystem, snapshots, and preview URLs. *(★ 1.1k)*
- [clawk](https://github.com/clawkwork/clawk) — Disposable Linux VM handed to a coding agent instead of the host machine. *(★ 1k, Apache-2.0)*
- [Tensorlake](https://www.tensorlake.ai) — Serverless Firecracker and Cloud Hypervisor sandboxes for durable agent loops. *(★ 1k, Apache-2.0)*
- [Wassette](https://microsoft.github.io/wassette/) — Runtime that serves WebAssembly components as MCP tools with capability limits. *(★ 955, MIT)*
- [InstaVM](https://instavm.io) — Firecracker microVM platform for code execution, previews, and persistent sessions. *(★ 893, Apache-2.0)*
- [Arrakis](https://github.com/abshkbh/arrakis) — Self-hosted Cloud Hypervisor microVMs for agent code and computer use, with checkpoint and backtrack. *(★ 882, AGPL-3.0)* 💤 dormant
- [code-on-incus](https://github.com/mensfeld/code-on-incus) — Gives each agent an Incus system container with its own systemd and Docker. *(★ 732, MIT)*
- [h5i](https://h5i.dev) — Per-agent sealed git worktrees so parallel coding agents do not share files, branches, or ports. *(★ 661, Apache-2.0)*
- [Yolobox](https://github.com/finbarr/yolobox) — Docker wrapper that runs coding agents with the host home directory unmounted. *(★ 646, MIT)*
- [SWE-ReX](https://swe-rex.com/) — Runtime that executes SWE-agent style coding sessions in remote sandboxes. *(★ 608, MIT)*
- [OpenComputer](https://opencomputer.dev) — Persistent Linux VMs for agents that hibernate when idle and support checkpoint and fork. *(★ 555, Apache-2.0)*
- [Modal Sandboxes](https://modal.com) — Modal's sandbox API runs untrusted code in gVisor-isolated containers, including GPU shapes. *(★ 518, Apache-2.0)*
- [sandboxed.sh](https://sandboxed.sh) — Orchestrator that isolates each agent mission in a systemd-nspawn container. *(★ 513)*
- [AgentBox](https://agent-box.sh) — Runs coding agents in parallel VMs via local Docker or a cloud sandbox provider. *(★ 499, MIT)*
- [Superserve](https://www.superserve.ai) — Firecracker sandboxes with unlimited session length, snapshots, and a credential broker. *(★ 464, Apache-2.0)*
- [amla-sandbox](https://github.com/amlalabs/amla-sandbox) — WebAssembly sandbox for agent code with a virtual filesystem and capability checks. *(★ 345)*
- [Capsule](https://github.com/capsulerun/runtime) — Executes agent tasks as untrusted code in isolated WebAssembly sandboxes. *(★ 297, Apache-2.0)*
- [ComputeSDK](https://www.computesdk.com) — Single SDK that dispatches sandbox calls across several hosted providers. *(★ 278, MIT)*
- [pctx](https://portofcontext.com) — Execution layer that runs untrusted code in type-checked Deno sandboxes. *(★ 278, MIT)*
- [Netclode](https://stanislas.blog/2026/02/netclode-self-hosted-cloud-coding-agent/) — Self-hosted coding-agent service using Kata Containers and Cloud Hypervisor. *(★ 256)*
- [Agent Sandbox Proxy](https://github.com/mattolson/agent-sandbox) — Docker sandbox whose outbound traffic passes through a proxy that injects secrets. *(★ 206, MIT)*
- [Vercel Sandbox](https://vercel.com/sandbox) — Firecracker microVMs on Vercel for untrusted code, with snapshots and a network firewall. *(★ 204, Apache-2.0)*
- [packnplay](https://github.com/obra/packnplay) — Launches coding agents in per-worktree Docker containers. *(★ 174)*
- [SandboxAI](https://github.com/substratusai/sandboxai) — Library that runs AI-generated Python and shell in Docker containers. *(★ 143)* 💤 dormant
- [clampdown](https://github.com/89luca89/clampdown) — Hardened container sandbox with an egress sidecar and an auth proxy that holds API keys. *(★ 116)*
- [vibebin](https://github.com/jgbrwn/vibebin) — Self-hosted Incus platform for persistent agent sandboxes with SSH routing. *(★ 108)*
- [Bouvet](https://deepwiki.com/vrn21/bouvet) — Rust sandbox for executing untrusted commands. *(★ 102, MIT)*
- [AgentVM](https://github.com/deepclause/agentvm) — Node.js library that runs an Alpine Linux image compiled to WebAssembly in a worker thread. *(★ 80, MIT)*
- [PocketEnv](https://pocketenv.io) — Local sandbox runtime intended for both agents and interactive use. *(★ 72, MPL-2.0)*
- [locki](https://github.com/JanPokorny/locki) — Lima and Incus sandbox that filters git operations from the agent. *(★ 68, Apache-2.0)*
- [HiveBox](https://tetiai.github.io/hivebox/) — Namespaces, cgroups, seccomp, and Landlock behind a CLI and REST API, one agent per sandbox. *(★ 61, BSD-3-Clause)*
- [clawker](https://docs.clawker.dev) — Self-hosted Docker sandboxes for coding agents behind an egress filter. *(★ 55, MIT)*
- [Kilntainers](https://kiln.tech) — MCP server that gives an agent an ephemeral Linux container for shell commands. *(★ 51, MIT)*
- [NovitaBox](https://novita.ai) — Local agent sandbox runtime with Firecracker, gVisor, and NVIDIA GPU sandbox modes. *(★ 48, Apache-2.0)*
- [PandaStack](https://www.pandastack.ai) — Open-source sandbox service for agents and code execution. *(★ 35, Apache-2.0)*
- [MCP Runner](https://mcp-runner-demo.tangier.io) — Runs MCP servers as ephemeral containers on the gVisor runtime. *(★ 32, Apache-2.0)*
- [Runloop](https://runloop.ai) — Hosted devboxes for coding agents, with snapshot and branch of sandbox state. *(★ 28, MIT)*
- [microsandbox-reef](https://reef.clawbits.ai) — Runs agents in microsandbox microVMs from a TOML role that sets image, domains, and secrets. *(★ 24, MIT)*
- [code-airlock](https://trivo25.github.io/code-airlock/) — Runs an unattended coding agent in a disposable microVM and commits its work for review. *(★ 21, MIT)*
- [Sandboxer](https://github.com/ammmir/sandboxer) — Self-hosted forkable server for running LLM and agent workloads. *(★ 21, MIT)* 💤 dormant
- [sand](https://github.com/banksean/sand) — Apple container CLI that clones a project into a disposable VM for a coding agent. *(★ 20, Apache-2.0)*
- [HyperAgent](https://github.com/hyperlight-dev/hyperagent) — Runs model-written JavaScript in Hyperlight microVMs with explicit host plugins. *(★ 19, Apache-2.0)*
- [ags](https://thomaspeklak.github.io/agent-sandbox/) — Rootless Podman CLI that runs coding agents in hardened containers. *(★ 16, MIT)*
- [container2wasm](https://github.com/ktock/container2wasm) — Converts a container image into a WebAssembly virtual machine image. *(★ 7, Apache-2.0)*
- [strangeClaw](https://github.com/itsthestranger/strangeClaw) — Self-hosted agent that can run inside Firecracker with a host-side request broker. *(★ 4, MIT)*
- [CreateOS](https://createos.sh) — MicroVMs with pause-to-snapshot, fork, and private overlay networking for multi-agent runs. *(★ 3, MIT)*
- [Baponi](https://baponi.ai) — nsjail sandboxes billed per execution, with object-storage mounts and an MCP server. *(★ 2, Apache-2.0)*
- [hort](https://johnsilverio.github.io/hort/) — Daemonless OCI sandbox plus a git worktree per agent. *(★ 2, AGPL-3.0)*
- [BunkerVM](https://ashishgituser.github.io/bunkervm/) — Firecracker microVMs that record each command and can rewind an agent run. *(★ 1, MIT)*
- [AgentSphere](https://www.agentsphere.run) — Hosted microVM sandboxes with an MCP interface for LLM code execution.
- [ainclave](https://ainclave.com) — Managed Firecracker microVMs with deny-by-default egress for agent workloads.
- [Blaxel](https://blaxel.ai) — Hosted microVM sandboxes that suspend when idle and resume with filesystem and memory state.
- [Box](https://box.ascii.dev) — Hosted Ubuntu VMs in the EU for agents, with SSH, fork, and desktop streaming.
- [CodeSandbox SDK](https://codesandbox.io) — MicroVM sandboxes with snapshot, restore, and live VM cloning, now part of Together AI.
- [Cognitora](https://www.cognitora.dev) — Hosted Firecracker microVMs marketed for hardware-isolated agent workloads.
- [Declaw](https://declaw.ai) — Firecracker sandboxes with network policy, TLS interception, and audit logging.
- [Docker Sandboxes](https://docs.docker.com/ai/sandboxes/) — Docker Desktop microVM sandboxes for coding agents, with a credential proxy and network policy.
- [exe.dev](https://exe.dev) — Hosted Ubuntu VMs aimed at coding agents, reachable over SSH.
- [Freestyle](https://freestyle.sh) — Hosted Linux VMs with sub-second provisioning, live fork, and pause/resume.
- [Islo](https://islo.dev) — Persistent Cloud Hypervisor microVMs for coding agents, with gateway profiles and BYOC.
- [Leap0](https://leap0.dev) — Hosted Firecracker microVMs with checkpoint, restore, and credential brokering.
- [Morph](https://morph.so) — VM infrastructure for agents with snapshot, restore, and environment branching.
- [Northflank Sandboxes](https://northflank.com) — MicroVM sandboxes on Kata, Firecracker, or gVisor, on Northflank cloud or in the customer's account.
- [Novita Agent Sandbox](https://novita.ai/sandbox) — Hosted agent sandboxes for code, desktop, and browser sessions, with an E2B-compatible SDK.
- [OmniRun](https://omnirun.io) — Hosted Firecracker microVMs for ephemeral agent runs, with a European region option.
- [Qbox](https://qbox.sh) — Self-hosted Firecracker orchestrator for agent sandboxes, with preview URLs and OCI templates.
- [shellbox.dev](https://shellbox.dev) — SSH-accessible hosted Linux boxes for agent and developer shells.
- [Sprites](https://sprites.dev) — Fly.io persistent Firecracker VMs with checkpoints, exec sessions, and egress policies.
- [VibeKit](https://docs.vibekit.sh) — SDK that starts coding-agent sessions on E2B, Daytona, Modal, and similar backends.

## MicroVMs & Hardware Isolation

*Firecracker-class microVMs and hardware-isolated environments for running untrusted agent work.*

- [Apple container](https://apple.github.io/container/documentation/) — Apple's container CLI that runs Linux containers as lightweight virtual machines on macOS. *(★ 50.4k, Apache-2.0)*
- [Firecracker](https://firecracker-microvm.github.io) — AWS KVM microVM monitor used to isolate untrusted workloads, including agent sandboxes. *(★ 37k, Apache-2.0)*
- [QEMU](https://www.qemu.org) — General machine emulator whose microvm machine type is used for fast lightweight guests. *(★ 13.8k)*
- [Kata Containers](https://katacontainers.io) — OCI runtime that executes each pod inside a VM, with QEMU, Cloud Hypervisor, and Firecracker hypervisors. *(★ 8.8k, Apache-2.0)*
- [KubeVirt](https://kubevirt.io) — Runs virtual machines as Kubernetes resources. *(★ 7.1k, Apache-2.0)*
- [smolvm](https://smolmachines.com) — libkrun microVM manager that runs OCI images on Linux and macOS and can fork a running VM. *(★ 6.4k, Apache-2.0)*
- [Cloud Hypervisor](https://www.cloudhypervisor.org) — Rust KVM hypervisor focused on cloud and microVM workloads. *(★ 6.3k)*
- [IncludeOS](https://includeos.github.io/) — Unikernel operating system for C++ network services. *(★ 5.2k, Apache-2.0)*
- [Harvester](https://harvesterhci.io) — Hyperconverged infrastructure that runs virtual machines on Kubernetes. *(★ 5.2k, Apache-2.0)*
- [Hyperlight](https://hyperlight.org) — Embeddable virtual machine monitor for running small guest functions in-process. *(★ 4.7k, Apache-2.0)*
- [arcbox](https://arcbox.dev) — Rust runtime that boots OCI images as isolated VMs for agents, locally first. *(★ 4.3k, Apache-2.0)*
- [OSv](https://osv.io) — Unikernel for running a single Linux binary in a virtual machine. *(★ 4.3k)*
- [Unikraft](https://unikraft.org) — Unikernel SDK that builds a specialized guest image for a single application. *(★ 3.9k)*
- [Nanos](https://nanovms.com) — Unikernel that runs one application as a virtual machine. *(★ 3.2k, Apache-2.0)*
- [MirageOS](https://mirage.io) — OCaml unikernel framework that compiles a service into a specialized guest. *(★ 3k, ISC)*
- [microvm.nix](https://microvm-nix.github.io/microvm.nix/) — NixOS modules for declaring microVMs on several hypervisors. *(★ 3k, MIT)*
- [firecracker-containerd](https://github.com/firecracker-microvm/firecracker-containerd) — Runs containerd workloads inside Firecracker microVMs. *(★ 2.9k, Apache-2.0)*
- [forkd](https://github.com/deeplethe/forkd) — Forks warm Firecracker microVMs so agent sandboxes can branch from a parent. *(★ 2.9k, Apache-2.0)*
- [libkrun](https://github.com/libkrun/libkrun) — Library that starts a KVM or Hypervisor.framework microVM to run a process. *(★ 2.7k, Apache-2.0)*
- [zeroboot](https://zeroboot.dev) — Copy-on-write forking of VM sandboxes aimed at sub-millisecond agent startup. *(★ 2.5k, Apache-2.0)*
- [BoxLite](https://boxlite.ai/) — Library that boots KVM or Hypervisor.framework microVMs and brokers secrets outside the guest. *(★ 2.4k, Apache-2.0)*
- [Gondolin](https://earendil-works.github.io/gondolin) — QEMU microVMs with a TypeScript control plane for agent sandboxes. *(★ 2.2k, Apache-2.0)*
- [Slim](https://github.com/ottomatica/slim) — Builds microVMs from Dockerfiles. *(★ 2.1k, Apache-2.0)* 💤 dormant
- [krunvm](https://github.com/libkrun/krunvm) — CLI for managing microVMs created with libkrun. *(★ 1.8k, Apache-2.0)*
- [libvirt](https://libvirt.org) — API and daemon for managing QEMU, KVM, and other virtual machine hypervisors. *(★ 1.7k, LGPL-2.1)*
- [Flintlock](https://flintlock.liquidmetal.dev/) — gRPC service that manages microVM lifecycle on top of containerd. *(★ 1.5k, MPL-2.0)*
- [Hermit](https://hermit-os.org) — Unikernel written in Rust for running a single application on a hypervisor. *(★ 1.5k, Apache-2.0)*
- [crosvm](https://crosvm.dev/book/) — ChromeOS virtual machine monitor, also used as a library for lightweight guest isolation. *(★ 1.3k, BSD-3-Clause)*
- [ACRN](https://projectacrn.github.io) — Hypervisor for embedded and partitioned workloads. *(★ 1.3k, BSD-3-Clause)*
- [Solo5](https://github.com/Solo5/solo5) — Sandboxed execution environment for unikernels on several hypervisors. *(★ 999, ISC)*
- [Fly Machines](https://fly.io/docs/machines/) — Fly.io Firecracker Machines API used to run persistent or ephemeral Linux VMs. *(★ 990)*
- [muvm](https://github.com/AsahiLinux/muvm) — Runs a Linux microVM on macOS via libkrun, used by Asahi and agent sandbox tools. *(★ 973)*
- [Vibe](https://github.com/lynaghk/vibe) — Boots Debian microVMs on macOS through Apple's Virtualization.framework for agent use. *(★ 957, MIT)*
- [shuru](http://shuru.run/) — Local-first microVM sandbox for running agents on macOS and Linux. *(★ 859, Apache-2.0)*
- [Xen](https://xenproject.org) — Type-1 hypervisor project, including a hypervisor-based isolation boundary. *(★ 852)*
- [Katakate](https://docs.katakate.org) — K3s distribution that runs workloads in Kata Containers on Firecracker. *(★ 810, Apache-2.0)*
- [firecracker-go-sdk](https://github.com/firecracker-microvm/firecracker-go-sdk) — Go SDK for driving the Firecracker API. *(★ 672, Apache-2.0)*
- [lkvm](https://github.com/kvmtool/kvmtool) — Lightweight KVM tool for booting a guest without QEMU. *(★ 645, GPL-2.0)*
- [firectl](https://github.com/firecracker-microvm/firectl) — Command-line launcher for Firecracker microVMs. *(★ 644, Apache-2.0)*
- [Matchlock](https://github.com/jingkaihe/matchlock) — CLI that runs agents in ephemeral Firecracker or Virtualization.framework microVMs with a secret-injecting proxy. *(★ 621, MIT)*
- [Virtink](https://github.com/smartxworks/virtink) — Kubernetes runtime that runs VM workloads with Cloud Hypervisor or QEMU. *(★ 611, Apache-2.0)*
- [gVisor tap vsock](https://github.com/containers/gvisor-tap-vsock) — User-space network stack used to connect microVMs without root on the host. *(★ 441, Apache-2.0)*
- [StratoVirt](https://github.com/openeuler-mirror/stratovirt) — openEuler Rust hypervisor for lightweight cloud VMs. *(★ 426)*
- [vfkit](https://github.com/crc-org/vfkit) — macOS command that starts Virtualization.framework virtual machines. *(★ 422, Apache-2.0)*
- [Alioth](https://github.com/google/alioth) — Google experimental virtual machine monitor written in Rust. *(★ 384, Apache-2.0)*
- [krunkit](https://github.com/libkrun/krunkit) — Tool for running libkrun microVMs on macOS. *(★ 368, Apache-2.0)*
- [Nehemiah](https://boringcomputers.com) — On-demand Firecracker Linux computers with a browser and terminal for agents. *(★ 333, Apache-2.0)*
- [urunc](https://urunc.io/) — Unikernel container runtime that boots unikernels through an OCI-compatible interface. *(★ 298, Apache-2.0)*
- [Cocoon](https://cocoonstack.github.io/cocoon/) — MicroVM engine on Cloud Hypervisor and Firecracker with OCI images, snapshots, and clones. *(★ 230, MIT)*
- [Brig](https://brig.sh) — Go CLI and daemon that run coding agents inside a microVM session. *(★ 187, Apache-2.0)*
- [libkrunfw](https://github.com/libkrun/libkrunfw) — Bundled guest kernel used by libkrun. *(★ 175)*
- [cluster-api-provider-microvm](https://github.com/liquidmetal-dev/cluster-api-provider-microvm) — Cluster API provider that provisions Kubernetes nodes as Flintlock microVMs. *(★ 158)*
- [pullrun](https://pullrun.dev) — Boots an OCI image as a Firecracker microVM, a container, or an Apple Silicon VM. *(★ 132, Apache-2.0)*
- [Cloud Hypervisor Rust VMM crates](https://github.com/rust-vmm/rust-vmm) — Shared Rust crates used to build microVM monitors such as Cloud Hypervisor and Firecracker. *(★ 107)*
- [brood-box](https://github.com/stacklok/brood-box) — Stacklok CLI that runs coding agents in hardware-isolated microVMs. *(★ 75, Apache-2.0)*
- [Cleanroom](https://github.com/buildkite/cleanroom) — Buildkite Firecracker microVMs with deny-by-default egress and host-side secret brokering. *(★ 67, MIT)*
- [Cocoon Sandbox](https://cocoonstack.github.io/sandbox/) — Warm-pooled microVM sandboxes for agents, built on the Cocoon VMM, with a no-network vsock mode. *(★ 61, AGPL-3.0)*
- [krunai](https://github.com/slp/krunai) — CLI that runs AI agents inside libkrun microVM sandboxes. *(★ 49, Apache-2.0)*
- [Chamber](https://github.com/cirruslabs/chamber) — Cirrus Labs tool for isolated VM sandboxes around agent and CI workloads. *(★ 46, AGPL-3.0)*
- [Cocoon Sandbox Operator](https://cocoonstack.github.io/sandbox-operator/) — Kubernetes front end and E2B-compatible API for warm Cocoon microVM pools. *(★ 42, AGPL-3.0)*
- [exec-sandbox](https://github.com/dualeai/exec-sandbox) — Python package that starts hardware-isolated VMs for untrusted code on the local machine. *(★ 38, Apache-2.0)*
- [go-microvm](https://github.com/stacklok/go-microvm) — Go library that runs OCI images as libkrun microVMs. *(★ 28, Apache-2.0)*
- [lingcage](https://lingcage.com) — Rust KVM VMM that clones microVMs to cage agent workloads. *(★ 21)*
- [drydock](https://sricola.github.io/drydock/) — Throwaway Apple container VMs for agent tasks, with deny-by-default egress. *(★ 8, Apache-2.0)*
- [AWS Lambda](https://aws.amazon.com/lambda/) — Serverless functions isolated in Firecracker microVMs, including snapshot resume.
- [bhyve](https://wiki.freebsd.org/bhyve) — FreeBSD hypervisor used to run lightweight virtual machines.
- [CubeSandbox](https://docs.cubesandbox.ai/) — Tencent KVM microVM sandbox with an E2B-compatible API and copy-on-write clones.
- [virtiofsd](https://gitlab.com/virtio-fs/virtiofsd) — Daemon that shares a host directory into a guest over virtio-fs.

## Code Execution APIs & Interpreters

*Hosted interpreter services and code-execution APIs agents call to run code.*

- [Node vm](https://nodejs.org/api/vm.html) — Node.js module that compiles and runs JavaScript in a new V8 context. *(★ 122.2k)*
- [V8 isolates](https://v8.dev/docs/embed) — V8 embedder API for running JavaScript in isolated heaps, the basis of Workers and isolated-vm. *(★ 25.3k)*
- [marimo](https://marimo.io) — Reactive Python notebook that executes cells in a local or hosted kernel. *(★ 22.9k, Apache-2.0)*
- [RustPython](https://rustpython.github.io) — Python interpreter written in Rust, embeddable as an in-process sandbox. *(★ 22.4k, MIT)*
- [MicroPython](https://micropython.org) — Small Python implementation that can run untrusted scripts on a microcontroller or in WebAssembly. *(★ 22.1k)*
- [Wasmer](https://wasmer.io) — WebAssembly runtime and edge platform for running sandboxed modules. *(★ 21.1k, MIT)*
- [Compiler Explorer](https://godbolt.org) — Runs compilers and can execute the resulting binary in a sandbox. *(★ 19.1k, BSD-2-Clause)*
- [Wasmtime](https://wasmtime.dev) — WebAssembly runtime used to execute untrusted code with capability limits. *(★ 18.7k, Apache-2.0)*
- [Windmill](https://www.windmill.dev) — Workflow engine that executes scripts and notebooks in isolated workers. *(★ 18.1k)*
- [IPython](https://ipython.org) — Interactive Python shell used as the default Jupyter kernel. *(★ 16.8k, BSD-3-Clause)*
- [Pyodide](https://pyodide.org) — CPython compiled to WebAssembly, used as an in-browser code interpreter. *(★ 14.9k, MPL-2.0)*
- [WasmEdge](https://wasmedge.org) — WebAssembly runtime aimed at cloud, edge, and plugin sandboxes. *(★ 10.8k, Apache-2.0)*
- [Monty](https://pydantic.dev/docs/monty/) — Minimal Python interpreter written in Rust with capability controls for untrusted code. *(★ 8.4k, MIT)*
- [JupyterHub](https://jupyter.org/hub) — Multi-user server that spawns a Jupyter notebook environment per person. *(★ 8.3k, BSD-3-Clause)*
- [wasm3](https://x.com/wasm3_engine) — Small WebAssembly interpreter. *(★ 8k, MIT)*
- [Apache Zeppelin](https://zeppelin.apache.org) — Web notebook that runs interpreters for several languages. *(★ 6.7k, Apache-2.0)*
- [evcxr](https://github.com/evcxr/evcxr) — Rust REPL and Jupyter kernel. *(★ 6.5k)*
- [Papermill](http://papermill.readthedocs.io/en/latest/) — Parameterizes and executes Jupyter notebooks. *(★ 6.5k, BSD-3-Clause)*
- [Wazero](https://wazero.io) — Zero-dependency WebAssembly runtime written in Go. *(★ 6.4k, Apache-2.0)*
- [Sandpack](https://sandpack.codesandbox.io) — In-browser bundler and runner for client-side code sandboxes. *(★ 6.2k, Apache-2.0)* 💤 dormant
- [WAMR](https://github.com/wasm-micro-runtime/wasm-micro-runtime) — Bytecode Alliance lightweight WebAssembly virtual machine for embedded and trusted execution. *(★ 6.1k, Apache-2.0)*
- [Voila](https://voila.readthedocs.io) — Turns a Jupyter notebook into a running web application. *(★ 5.9k)*
- [Extism](https://extism.org) — SDK for embedding WebAssembly plugins as a sandbox inside a host application. *(★ 5.8k, BSD-3-Clause)*
- [Pluto.jl](https://plutojl.org) — Reactive Julia notebook that re-runs dependent cells. *(★ 5.4k, MIT)*
- [JupyterLite](https://jupyterlite.readthedocs.io) — Jupyter distribution that runs kernels in the browser via WebAssembly. *(★ 4.9k, BSD-3-Clause)*
- [Lunatic](https://lunatic.solutions) — Erlang-inspired runtime that isolates WebAssembly processes. *(★ 4.9k, Apache-2.0)* 💤 dormant
- [Polynote](https://polynote.org) — Polyglot notebook from Netflix with a shared kernel. *(★ 4.6k, Apache-2.0)*
- [Judge0](https://judge0.com) — Sandboxed online code execution system used by apps and by agents. *(★ 4.5k, GPL-3.0)*
- [just-bash](https://justbash.dev/) — Bash interpreter implemented in JavaScript for sandboxed agent shells. *(★ 4.3k)*
- [vm2](https://github.com/patriksimek/vm2) — Node.js sandbox library; the repository is discontinued after multiple escapes. *(★ 4.1k, MIT)*
- [QuickJS-ng](https://quickjs-ng.github.io/quickjs/) — Embeddable JavaScript engine used to run untrusted scripts in-process. *(★ 3.8k, MIT)*
- [isolated-vm](https://github.com/laverdet/isolated-vm) — Node.js library that runs JavaScript in a separate V8 isolate with memory limits. *(★ 2.9k, ISC)*
- [BeakerX](http://BeakerX.com) — Collection of Jupyter kernels and widgets for polyglot notebooks. *(★ 2.9k, Apache-2.0)* 💤 dormant
- [Piston](https://emkc.org/run) — High-performance code execution engine that isolates each run. *(★ 2.8k, MIT)*
- [E2B Code Interpreter](https://e2b.dev/?utm_source=github&utm_medium=referral&utm_campaign=repo_website&utm_content=code-interpreter) — E2B template and SDK that exposes a Jupyter-style code interpreter inside a sandbox. *(★ 2.4k, Apache-2.0)*
- [wasmi](https://wasmi-labs.github.io/wasmi/) — WebAssembly interpreter written in Rust. *(★ 2.3k, Apache-2.0)*
- [Codapi](https://codapi.org) — Self-hosted code execution widget and API with sandbox backends. *(★ 2.1k, Apache-2.0)*
- [fengari](https://github.com/fengari-lua/fengari) — Lua VM implemented in JavaScript for sandboxed scripting. *(★ 2k, MIT)*
- [Glot](https://glot.io/) — Pastebin-style code runner with per-language Docker sandboxes. *(★ 1.7k)* 💤 dormant
- [GraalPy](https://www.graalvm.org/python/) — Python implementation on GraalVM used to embed a restricted interpreter. *(★ 1.6k)*
- [isolate](https://github.com/ioi/isolate) — IOI sandbox that runs a program under cgroups, namespaces, and system-call filters. *(★ 1.5k)*
- [DMOJ](https://dmoj.ca) — Online-judge platform with an isolated code execution backend. *(★ 1.2k, AGPL-3.0)*
- [llm-sandbox](https://vndee.github.io/llm-sandbox/) — Python library that executes LLM-generated code on Docker, Podman, or Kubernetes. *(★ 1.1k, MIT)*
- [Observable](https://observablehq.com) — Reactive JavaScript notebooks that execute in the browser and on Observable servers. *(★ 1.1k, ISC)*
- [Endo](https://endojs.org/) — Hardened JavaScript SES lockdown used to confine guest code. *(★ 1.1k, Apache-2.0)*
- [xeus](https://xeus.readthedocs.io/) — C++ library for writing Jupyter kernels. *(★ 963, BSD-3-Clause)*
- [Faasm](https://faasm.readthedocs.io) — Distributed runtime that executes functions as WebAssembly with a shared state API. *(★ 926, Apache-2.0)*
- [DOMjudge](https://www.domjudge.org) — Programming-contest judge that executes submissions in a sandbox. *(★ 916, GPL-2.0)*
- [Jupyter Enterprise Gateway](https://jupyter-enterprise-gateway.readthedocs.io/en/latest/) — Launches Jupyter kernels in distributed containers or clusters. *(★ 668)*
- [Jupyter Kernel Gateway](http://jupyter-kernel-gateway.readthedocs.org/en/latest/) — HTTP and WebSocket service in front of Jupyter kernels. *(★ 563)* 💤 dormant
- [Xeus-Python](https://github.com/jupyter-xeus/xeus-python) — Jupyter kernel for Python built on xeus. *(★ 480, BSD-3-Clause)*
- [Thebe](https://thebe.readthedocs.io) — Turns static code cells on a web page into live Jupyter kernel sessions. *(★ 442, BSD-3-Clause)*
- [CodeBoxAPI](https://codeboxapi.com) — Small sandbox service for executing code produced by LLM applications. *(★ 363, MIT)* 💤 dormant
- [Suborbital Sat](https://github.com/suborbital/sat) — WebAssembly function runner from the former Suborbital project. *(★ 351, Apache-2.0)* 💤 dormant
- [mcp-server-code-execution-mode](https://github.com/elusznik/mcp-server-code-execution-mode) — MCP server that executes Python in rootless containers. *(★ 340, GPL-3.0)*
- [bots-garden Capsule](https://bots-garden.github.io/capsule/) — WebAssembly runner for server-side functions with host capability limits. *(★ 292, MIT)* 💤 dormant
- [nteract](https://github.com/nteract/nteract) — Desktop and library notebook client that executes code through Jupyter kernels. *(★ 176, BSD-3-Clause)*
- [LocalSandbox](https://github.com/coplane/localsandbox) — In-process bash and Python environment built from a virtual filesystem and Pyodide. *(★ 158)*
- [Eryx](https://github.com/eryx-org/eryx) — Runs CPython on Wasmtime with memory and CPU limits and no filesystem or network by default. *(★ 76, Apache-2.0)*
- [codeinterpreter-codebox](https://github.com/zhangzhejian/codeinterpreter-codebox) — Deployable Python code-interpreter sandbox service. *(★ 57, MIT)* 💤 dormant
- [Enclave](https://enclave.agentfront.dev) — JavaScript sandbox that blocks prototype pollution and host access for untrusted scripts. *(★ 6, Apache-2.0)*
- [pctx-py-sandbox](https://portofcontext.com) — Python decorator that executes untrusted code outside the caller process. *(★ 5, MIT)*
- [PythonSafeEval](https://github.com/s3131212/PythonSafeEval) — Executes Python inside nsjail in a Docker container. *(★ 5, MIT)* 💤 dormant
- [bashkit4j](https://central.sonatype.com/artifact/io.github.terseprompts/bashkit4j) — In-JVM bash implementation with an in-memory filesystem for untrusted agent scripts. *(★ 3, MIT)*
- [scriptling](https://scriptling.dev/) — Small embeddable interpreter for agent-written scripts. *(★ 2, MIT)*
- [Anthropic Code Execution](https://docs.anthropic.com/en/docs/agents-and-tools/tool-use/code-execution-tool) — Anthropic tool that runs Bash and file operations in a hosted sandbox.
- [Azure Dynamic Sessions](https://learn.microsoft.com/en-us/azure/container-apps/sessions) — Azure Container Apps pool of sandboxes for code interpreter and custom containers.
- [Bedrock AgentCore Code Interpreter](https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/code-interpreter-tool.html) — Amazon Bedrock AgentCore tool that executes code in a managed sandbox.
- [Deepnote](https://deepnote.com) — Collaborative hosted notebooks with a machine per project.
- [Deno](https://deno.com) — JavaScript runtime with permission flags that deny file, network, and environment access by default.
- [Fastly Compute](https://www.fastly.com/products/compute) — Wasmtime-based edge platform that runs untrusted WebAssembly applications.
- [Gemini Code Execution](https://ai.google.dev/gemini-api/docs/code-execution) — Gemini API tool that executes Python generated by the model.
- [Google Colab](https://colab.research.google.com) — Hosted Jupyter notebooks with optional paid compute.
- [Hex](https://hex.tech) — Hosted notebook and data app environment that runs Python and SQL.
- [interpretthis](https://github.com/moderately-ai/interpretthis) — Sandboxed Python AST interpreter for untrusted model output. *(Apache-2.0)*
- [JDoodle](https://www.jdoodle.com) — Online compiler with a code-execution API.
- [JetBrains Datalore](https://datalore.jetbrains.com) — JetBrains hosted and on-prem Jupyter notebooks.
- [Kaggle Kernels](https://www.kaggle.com/code) — Hosted notebooks that execute Python and R on Kaggle.
- [Nextjournal](https://nextjournal.com) — Notebook environment that runs code with reproducible environments.
- [OneCompiler](https://onecompiler.com) — Browser compiler with an API for running code in many languages.
- [OpenAI Code Interpreter](https://platform.openai.com/docs/guides/tools-code-interpreter) — OpenAI tool that executes Python in a hosted sandbox attached to a model response.
- [Paiza.IO](https://paiza.io) — Online IDE and code-execution service.
- [Sphere Engine](https://sphere-engine.com) — Commercial code-execution API used by education and assessment products.
- [Val Town](https://www.val.town) — Hosted JavaScript and TypeScript functions with HTTP endpoints.
- [Wandbox](https://wandbox.org) — Online compiler and code runner with saved snippets.
- [WebContainers](https://webcontainers.io) — Node.js runtime that executes inside the browser's security sandbox.

## Cloud Workspaces & Dev Environments

*Cloud dev boxes, workspace managers, and git-worktree environments agents develop inside.*

- [code-server](https://coder.com/docs/code-server) — VS Code running in the browser on a remote machine. *(★ 79.5k, MIT)*
- [Lightning AI Studios](https://lightning.ai) — Hosted studios for Python and ML workloads with persistent machines. *(★ 31.4k, Apache-2.0)*
- [Colima](https://colima.run) — macOS wrapper that provides a Docker or containerd runtime inside a Lima VM. *(★ 31k, MIT)*
- [Lima](https://lima-vm.io) — Linux virtual machines on macOS, used as local dev boxes and container hosts. *(★ 22k, Apache-2.0)*
- [Coder](https://coder.com) — Self-hosted platform that provisions per-user development environments. *(★ 16.7k, AGPL-3.0)*
- [DevPod](https://devpod.sh) — Client-only tool that creates devcontainer workspaces on a laptop or any cloud. *(★ 15.2k, MPL-2.0)*
- [Ona](https://ona.com) — Cloud development environments, formerly Gitpod, used as remote workspaces for agents. *(★ 13.8k, AGPL-3.0)*
- [distrobox](https://distrobox.it) — Creates pet containers that share the host home directory, used as per-project dev boxes. *(★ 13k, GPL-3.0)*
- [Devbox](https://www.jetify.com/devbox) — Nix-based isolated development environment declared in a json file. *(★ 12.4k, Apache-2.0)*
- [Multipass](https://canonical.com/multipass) — Canonical CLI that launches Ubuntu virtual machines on macOS, Windows, and Linux. *(★ 9.3k, GPL-3.0)*
- [Telepresence](https://telepresence.io) — Proxies a local process into a remote Kubernetes cluster for development. *(★ 7.3k, Apache-2.0)*
- [Eclipse Che](https://www.eclipse.org/che/) — Kubernetes-native cloud IDE and workspace server. *(★ 7.2k, EPL-2.0)*
- [openvscode-server](https://www.gitpod.io/) — Server build of VS Code used inside browser-based cloud workspaces. *(★ 6.2k, MIT)*
- [mirrord](https://mirrord.dev) — Runs a local process in the context of a remote Kubernetes pod. *(★ 5.3k, MIT)*
- [StackBlitz](https://stackblitz.com) — Browser IDE whose WebContainer API runs Node.js inside the browser sandbox. *(★ 4.6k, MIT)* 💤 dormant
- [Flox](https://flox.dev) — Nix-based virtual environments for projects, with optional remote environments. *(★ 4.1k, GPL-2.0)*
- [Garden](https://garden.io) — Development and preview-environment tool for Kubernetes applications. *(★ 3.6k, MPL-2.0)*
- [Okteto](https://www.okteto.com) — Remote development and preview environments on Kubernetes. *(★ 3.5k, Apache-2.0)*
- [Toolbx](https://containertoolbx.org) — Fedora pet-container tool for mutable development environments on immutable hosts. *(★ 3.5k, Apache-2.0)*
- [devcontainers CLI](https://containers.dev) — Reference CLI that builds and starts a Development Container from devcontainer.json. *(★ 3k, MIT)*
- [Uffizzi](https://www.uffizzi.com) — Virtual clusters and preview environments for pull requests. *(★ 354, Apache-2.0)* 💤 dormant
- [Qovery](https://www.qovery.com) — Platform that runs preview environments and an agent task runner next to applications. *(★ 227, GPL-3.0)*
- [Bunnyshell](https://www.bunnyshell.com) — Ephemeral environments built from a repository definition. *(★ 17, MIT)*
- [machine](https://runmachine.dev) — One Lima VM per GitHub project, with no host filesystem mounted. *(★ 15, MIT)*
- [Amazon SageMaker Studio](https://aws.amazon.com/sagemaker/ai/studio/) — AWS IDE and notebook environment for ML development.
- [AWS Cloud9](https://aws.amazon.com/cloud9/) — Browser IDE on an EC2 instance.
- [Brev](https://brev.nvidia.com) — NVIDIA product for launching GPU development environments.
- [Coherence](https://www.withcoherence.com) — Preview environments and full-stack hosting tied to pull requests.
- [DevZero](https://www.devzero.io) — Remote development environments with microVM isolation.
- [Domino Data Lab](https://domino.ai) — Enterprise platform that runs data-science workspaces and jobs.
- [Firebase Studio](https://firebase.studio) — Google's browser workspace for full-stack apps, evolved from Project IDX.
- [GitHub Codespaces](https://github.com/features/codespaces) — GitHub-hosted dev containers attached to a repository.
- [GitLab Workspaces](https://docs.gitlab.com/user/workspace/) — GitLab remote development environments running in a Kubernetes cluster.
- [Google Cloud Workstations](https://cloud.google.com/workstations) — Managed development environments on Google Cloud.
- [JetBrains CodeCanvas](https://www.jetbrains.com/codecanvas/) — JetBrains self-hosted development-environment platform.
- [JetBrains Gateway](https://www.jetbrains.com/remote-development/) — Thin client that connects a JetBrains IDE to a remote development machine.
- [Namespace](https://namespace.so) — Remote preview and development environments for repositories.
- [OpenShift Dev Spaces](https://developers.redhat.com/products/openshift-dev-spaces/overview) — Red Hat distribution of cloud workspaces based on Eclipse Che.
- [OrbStack](https://orbstack.dev) — macOS app that runs Linux machines and containers on a lightweight hypervisor.
- [Paperspace Gradient](https://www.paperspace.com/gradient) — DigitalOcean notebooks and machines for ML development.
- [Posit Workbench](https://posit.co/products/enterprise/workbench/) — Posit server for RStudio, Jupyter, and VS Code sessions.
- [Release](https://release.com) — Ephemeral environments created per pull request.
- [Replit](https://replit.com) — Hosted programming environment with a persistent container per project.
- [SageMaker Studio Code Editor](https://docs.aws.amazon.com/sagemaker/latest/dg/code-editor.html) — VS Code-based editor inside Amazon SageMaker Studio spaces.
- [Saturn Cloud](https://saturncloud.io) — Hosted environments for data-science notebooks and jobs.
- [Signadot](https://www.signadot.com) — Sandbox environments that fork a subset of a Kubernetes stack per change.
- [Strong Network](https://www.strong.network) — Enterprise cloud development environments with network isolation.
- [Vertex AI Workbench](https://cloud.google.com/vertex-ai/docs/workbench/introduction) — Google Cloud Jupyter notebooks on managed virtual machines.

## Agent Hosting & Deployment

*Platforms that deploy and keep agents running — agent clouds, hosting, and persistent runtimes.*

- [Dify](https://dify.ai) — Platform for building and hosting LLM applications and agents. *(★ 157.4k)*
- [Langflow](https://www.langflow.org) — Visual builder and server for deploying agent flows. *(★ 155.3k, MIT)*
- [CrewAI AMP](https://crewai.com) — CrewAI's managed control plane for deploying crews. *(★ 59.2k, MIT)*
- [Flowise](https://flowiseai.com) — Low-code server for deploying LLM flows and agents. *(★ 55.5k)*
- [LangGraph Platform](https://langchain-ai.github.io/langgraph/concepts/langgraph_platform/) — Hosted and self-hosted runtime for deploying LangGraph agents. *(★ 42.4k, MIT)*
- [Agno](https://www.agno.com) — Agent runtime, formerly Phidata, with a control plane for running agents. *(★ 42.4k, Apache-2.0)*
- [FastGPT](https://fastgpt.io) — Self-hostable platform for knowledge-base agents and workflows. *(★ 29.8k)*
- [Mastra](https://mastra.ai) — TypeScript agent framework with a cloud for deploying agents. *(★ 28.4k)*
- [Letta](https://www.letta.com) — Stateful agent server you can self-host or run on Letta Cloud. *(★ 25k, Apache-2.0)*
- [Botpress](https://botpress.com) — Platform for building and hosting conversational agents. *(★ 14.9k, MIT)*
- [workerd](https://blog.cloudflare.com/workerd-open-source-workers-runtime/) — Cloudflare Workers runtime that isolates scripts in V8 isolates. *(★ 8.8k, Apache-2.0)*
- [Superagent](https://www.superagent.sh) — Open-source runtime and cloud for deploying agents with tools. *(★ 6.8k, MIT)*
- [Spin](https://www.fermyon.com/spin) — Fermyon framework that runs WebAssembly applications as isolated serverless units. *(★ 6.5k, Apache-2.0)*
- [PartyKit](https://www.partykit.io) — Hosted realtime rooms on Cloudflare Durable Objects, used for collaborative agents. *(★ 5.7k, MIT)*
- [Cloudflare Agents](https://developers.cloudflare.com/agents/) — SDK for long-lived agents on Cloudflare Durable Objects. *(★ 5.7k, MIT)*
- [wasmCloud](https://wasmcloud.com) — Distributed runtime that runs WebAssembly components with explicit capabilities. *(★ 2.4k, Apache-2.0)*
- [Dust](https://dust.tt) — Hosted workspace for company agents connected to internal tools. *(★ 1.5k, MIT)*
- [Atmo](https://suborbital.dev) — Suborbital server that routed HTTP to WebAssembly functions. *(★ 720, Apache-2.0)* 💤 dormant
- [Agent Machines](https://agent-machines.dev) — Control plane that provisions persistent agent workers onto selectable sandbox substrates. *(★ 31, MIT)*
- [Amazon Bedrock AgentCore](https://aws.amazon.com/bedrock/agentcore/) — AWS runtime for deploying agents, with a browser, code interpreter, and memory services.
- [Azure AI Agent Service](https://learn.microsoft.com/en-us/azure/ai-services/agents/overview) — Azure service for hosting agents with tool and code-interpreter sessions.
- [Coze](https://www.coze.com) — ByteDance hosted builder and runtime for bots and agents.
- [Fermyon Cloud](https://www.fermyon.com/cloud) — Managed host for Spin WebAssembly applications.
- [Fixie](https://www.fixie.ai) — Platform for deploying conversational agents, later focused on voice.
- [Gumloop](https://www.gumloop.com) — Hosted automation platform that runs agent workflows.
- [MindStudio](https://www.mindstudio.ai) — Hosted builder for AI agents and tools.
- [Relevance AI](https://relevanceai.com) — Hosted platform for building and operating agents on business tools.
- [Stack AI](https://www.stack-ai.com) — Hosted builder that deploys agents as APIs and interfaces.
- [Steamship](https://www.steamship.com) — Hosted runtime and SDK for packaging agents as web services.
- [Vertex AI Agent Engine](https://cloud.google.com/vertex-ai/generative-ai/docs/agent-engine/overview) — Google Cloud runtime for deploying and scaling agents.
- [Voiceflow](https://www.voiceflow.com) — Hosted design and runtime platform for conversational agents.
- [Wasmer Edge](https://wasmer.io/products/edge) — Wasmer's edge network for deploying WebAssembly applications.
- [Wordware](https://www.wordware.ai) — Hosted environment for authoring and running natural-language agent programs.

## Computer-Use VMs & Desktop Sandboxes

*Full desktop/VM environments for computer-use and GUI-driving agents.*

- [UTM](https://mac.getutm.app) — QEMU and Apple Virtualization frontend for desktop virtual machines on macOS and iOS. *(★ 35.7k, Apache-2.0)*
- [Cua](https://cua.ai) — Open-source computer-use stack with local and cloud desktop sandboxes for Linux, macOS, Windows, and Android. *(★ 26.9k, MIT)*
- [Anthropic Computer Use Demo](https://docs.anthropic.com/en/docs/agents-and-tools/tool-use/computer-use-tool) — Reference Docker desktop with Xvfb, a window manager, and Firefox for the computer-use tool. *(★ 17.8k, MIT)*
- [quickemu](https://github.com/quickemu-project/quickemu) — Downloads and launches desktop guest images under QEMU with little configuration. *(★ 16.4k, MIT)*
- [docker-android](https://github.com/budtmo/docker-android) — Android emulator packaged in Docker, with VNC and ADB access. *(★ 15.9k)*
- [noVNC](https://novnc.com) — Browser VNC client used to view and drive agent desktops. *(★ 14.1k)*
- [Waydroid](https://waydro.id) — Runs Android in a container on a Linux desktop using the host kernel. *(★ 12.3k, GPL-3.0)*
- [TigerVNC](https://tigervnc.org) — VNC client and server used to export a virtual desktop. *(★ 7.5k, GPL-2.0)*
- [Tart](https://tart.run) — Virtualizes macOS and Linux on Apple silicon for CI and agent fleets. *(★ 7.2k)*
- [redroid](https://github.com/remote-android/redroid-doc) — Android in a container, used as a remote device for agents. *(★ 6.9k)*
- [KasmVNC](https://github.com/kasmtech/KasmVNC) — Web-native VNC server used to expose a desktop to remote agents. *(★ 5.3k, GPL-2.0)*
- [linuxserver webtop](https://github.com/linuxserver/docker-webtop) — Docker images that serve a full Linux desktop in the browser. *(★ 4.4k, GPL-3.0)*
- [OSWorld](https://os-world.github.io) — Desktop environment and benchmark that runs computer-use tasks in virtual machines. *(★ 3.2k, Apache-2.0)*
- [E2B Desktop](https://e2b.dev/?utm_source=github&utm_medium=referral&utm_campaign=repo_website&utm_content=desktop) — E2B sandbox image with a Linux desktop that an agent can screenshot and click. *(★ 1.5k, Apache-2.0)*
- [AndroidEnv](https://github.com/google-deepmind/android_env) — DeepMind library that exposes an Android emulator as an agent environment. *(★ 1.2k, Apache-2.0)*
- [Kasm Workspaces](https://kasm.com) — Streams containerized desktops and browsers to a browser client. *(★ 1.2k)*
- [AndroidWorld](https://github.com/google-research/android_world) — Android emulator environment for agents that operate mobile apps. *(★ 936, Apache-2.0)*
- [WindowsAgentArena](https://microsoft.github.io/WindowsAgentArena) — Microsoft environment that evaluates computer-use agents inside Windows virtual machines. *(★ 904, MIT)*
- [OSWorld-V2](https://osworld-v2.xlang.ai) — Longer-horizon desktop task environments extending OSWorld. *(★ 339, Apache-2.0)*
- [bromure](https://bromure.io) — macOS app that opens a disposable Linux VM for browsing and coding agents. *(★ 293, MIT)*
- [GNOME Boxes](https://apps.gnome.org/Boxes/) — Simple GNOME application for running desktop virtual machines. *(★ 181)*
- [nilbox](https://nilbox.run) — Desktop app that gives each project a Linux VM and keeps tokens on the host. *(★ 16, GPL-3.0)*
- [Android Emulator](https://developer.android.com/studio/run/emulator) — Official Android virtual device used by mobile computer-use environments.
- [Anka](https://veertu.com) — Veertu's macOS virtualization platform for build and agent fleets.
- [appetize](https://appetize.io) — Streams Android and iOS simulators in the browser.
- [Corellium](https://www.corellium.com) — Virtual iOS and Android devices for security research.
- [Genymotion](https://www.genymotion.com) — Android virtual devices in the cloud and on the desktop.
- [Hyper-V](https://learn.microsoft.com/en-us/virtualization/hyper-v-on-windows/about/) — Windows hypervisor used for local desktop and container isolation.
- [Manus Cloud Computer](https://manus.im) — Persistent Ubuntu computer attached to the Manus agent.
- [Orgo](https://orgo.ai) — Hosted virtual desktops intended for computer-use agents.
- [Parallels Desktop](https://www.parallels.com/products/desktop/) — macOS desktop hypervisor for Windows and Linux guests.
- [Proxmox VE](https://www.proxmox.com/en/products/proxmox-virtual-environment/overview) — Debian-based host for KVM virtual machines and LXC containers.
- [Scrapybara](https://scrapybara.com) — Hosted Linux desktop instances for computer-use agents.
- [VirtualBox](https://www.virtualbox.org) — Cross-platform desktop hypervisor used for local agent guests.
- [VMware Fusion](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion) — Desktop hypervisor for macOS hosts, used by OSWorld's macOS provider.
- [VMware Workstation](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion) — Broadcom desktop hypervisor for Windows and Linux guests.
- [Windows Sandbox](https://learn.microsoft.com/en-us/windows/security/application-security/application-isolation/windows-sandbox/) — Disposable Windows desktop that discards its state when the window closes.

## Isolation Utilities & SDKs

*SDKs, CLIs, and glue for wrapping agent processes in isolation.*

- [Docker Engine](https://docs.docker.com/engine/) — Container engine whose containers are the default isolation boundary in many agent sandboxes. *(★ 72.1k, Apache-2.0)*
- [Podman](https://podman.io) — Daemonless container engine that can run rootless containers for agent sandboxes. *(★ 33k, Apache-2.0)*
- [containerd](https://containerd.io) — Container runtime core used under Docker and Kubernetes, with pluggable sandbox controllers. *(★ 21.3k, Apache-2.0)*
- [Sandboxie-Plus](https://sandboxie-plus.com) — Windows sandbox that redirects an application's file and registry writes. *(★ 19.6k, GPL-3.0)*
- [gVisor](https://gvisor.dev) — User-space kernel that intercepts syscalls from a container, shipped as the runsc OCI runtime. *(★ 19.4k, Apache-2.0)*
- [Nix](https://nixos.org) — Package manager whose build sandbox isolates compilers from the host filesystem and network. *(★ 17.8k, LGPL-2.1)*
- [systemd-nspawn](https://www.freedesktop.org/software/systemd/man/systemd-nspawn.html) — systemd tool that boots a directory or image as a lightweight container. *(★ 16.8k, GPL-2.0)*
- [runc](https://www.opencontainers.org/) — Reference OCI container runtime that creates Linux containers. *(★ 13.5k, Apache-2.0)*
- [nerdctl](https://github.com/containerd/nerdctl) — Docker-compatible CLI for containerd, including rootless mode. *(★ 10.4k, Apache-2.0)*
- [NVIDIA OpenShell](https://docs.nvidia.com/openshell/latest/) — Agent runtime that applies declarative file, network, and process policy to a container. *(★ 9.5k, Apache-2.0)*
- [bubblewrap](https://github.com/containers/bubblewrap) — Unprivileged sandbox tool that creates a new user, mount, and network namespace for a process. *(★ 8.9k)*
- [firejail](https://firejail.wordpress.com) — SUID sandbox that restricts Linux applications with namespaces and seccomp. *(★ 7.7k, GPL-2.0)*
- [youki](https://youki-dev.github.io/youki/) — Rust implementation of the OCI container runtime. *(★ 7.6k, Apache-2.0)*
- [Incus](https://linuxcontainers.org/incus) — System container and virtual machine manager forked from LXD. *(★ 6.3k, Apache-2.0)*
- [CRI-O](https://cri-o.io) — Kubernetes CRI runtime that launches OCI containers. *(★ 5.7k, Apache-2.0)*
- [Anthropic Sandbox Runtime](https://github.com/anthropics/sandbox-runtime) — Filesystem and network sandbox used by Claude Code, via Seatbelt on macOS and bubblewrap on Linux. *(★ 5.4k, Apache-2.0)*
- [LXC](https://linuxcontainers.org/lxc) — Low-level Linux container runtime that gives a guest its own init. *(★ 5.3k)*
- [Flatpak](https://flatpak.org) — Desktop application sandbox using bubblewrap, namespaces, and seccomp. *(★ 5.1k, LGPL-2.1)*
- [LXD](https://canonical.com/lxd) — Canonical's system container and VM manager, still used for per-agent machines. *(★ 4.8k, AGPL-3.0)*
- [nono](https://nono.sh) — Capability-based sandbox for agent commands using Landlock on Linux and Seatbelt on macOS. *(★ 4.3k, Apache-2.0)*
- [crun](https://github.com/containers/crun) — Fast C OCI runtime used by Podman and by several agent sandbox stacks. *(★ 4.1k, GPL-2.0)*
- [nsjail](https://nsjail.dev) — Process jail using Linux namespaces, cgroups, and seccomp, widely used for code execution. *(★ 4.1k, Apache-2.0)*
- [Sysbox](https://github.com/nestybox/sysbox) — OCI runtime that lets a container run systemd and nested containers without a privileged daemon. *(★ 3.9k, Apache-2.0)*
- [AgentFS](https://www.agentfs.ai) — Copy-on-write filesystem for agents stored in a SQLite database. *(★ 3.4k)*
- [proot](https://proot-me.github.io) — User-space chroot and mount emulation via ptrace, used where namespaces are unavailable. *(★ 2.6k, GPL-2.0)*
- [Landrun](https://github.com/Zouuup/landrun) — Unprivileged Landlock runner that confines a Linux process without root. *(★ 2.3k, MIT)*
- [Apptainer](https://apptainer.org) — Container runtime for unprivileged HPC workloads, formerly Singularity. *(★ 2k)*
- [Sandboxed API](https://developers.google.com/sandboxed-api/) — Google library for running C and C++ code inside a sandboxed process, including the Sandbox2 helper. *(★ 1.8k, Apache-2.0)*
- [Occlum](https://occlum.io/) — Memory-safe library OS for running applications inside Intel SGX enclaves. *(★ 1.5k)*
- [Enarx](https://enarx.dev/) — WebAssembly runtime that executes workloads inside hardware enclaves. *(★ 1.4k, Apache-2.0)*
- [ai-jail](https://github.com/akitaonrails/ai-jail) — Bubblewrap, Landlock, and Seatbelt profiles for coding-agent commands. *(★ 1.3k, GPL-3.0)*
- [rootlesskit](https://github.com/rootless-containers/rootlesskit) — Sets up a user-namespace network and mount environment for rootless containers. *(★ 1.3k, Apache-2.0)*
- [LavaMoat](https://lavamoat.github.io/) — Tools that confine JavaScript supply-chain code with SES compartments. *(★ 1.2k, MIT)*
- [Enroot](https://github.com/NVIDIA/enroot) — NVIDIA tool that turns a container image into an unprivileged sandbox for HPC jobs. *(★ 1.1k, Apache-2.0)*
- [SingularityCE](https://sylabs.io/docs/) — Sylabs container runtime for scientific and unprivileged sandboxed jobs. *(★ 995)*
- [Fence](https://fencesandbox.com/docs) — Container-free CLI that applies filesystem and network limits to a process. *(★ 981, Apache-2.0)*
- [Gramine](https://gramineproject.io) — Library OS that runs an unmodified binary inside an enclave or a Linux sandbox. *(★ 775, LGPL-3.0)*
- [hcsshim](https://github.com/microsoft/hcsshim) — Go interface to Windows Host Compute Service used to run process-isolated and Hyper-V containers. *(★ 695, MIT)*
- [Edgeless EGo](https://www.edgeless.systems/products/ego/) — Framework for running Go services inside Intel SGX enclaves. *(★ 595, MPL-2.0)*
- [Leash](https://leash.strongdm.ai/) — Wraps coding agents and enforces Cedar policies on their commands. *(★ 591, Apache-2.0)*
- [sandlock](https://sandlock.io) — Confines a process with Landlock, seccomp-bpf, and a copy-on-write working directory. *(★ 526, Apache-2.0)*
- [kern](https://getkern.dev) — Rootless daemonless container runtime positioned for agent tool calls and code execution. *(★ 428, Apache-2.0)*
- [Confidential Containers](https://confidentialcontainers.org) — Kubernetes project that runs pods inside confidential or hardware-isolated virtual machines. *(★ 401, Apache-2.0)*
- [minijail](https://google.github.io/minijail/) — ChromeOS and Android sandbox library for seccomp, capabilities, and namespaces. *(★ 386, BSD-3-Clause)*
- [Contrast](https://docs.edgeless.systems/contrast) — Confidential Kubernetes runtime from Edgeless Systems. *(★ 315)*
- [Greywall](https://greywall.io) — Container-free deny-by-default sandbox for filesystem, network, and syscalls. *(★ 305, Apache-2.0)*
- [MarbleRun](https://marblerun.sh) — Control plane for confidential microservices running in enclaves. *(★ 279)*
- [ClaudeCage](https://github.com/PACHAKUTlQ/ClaudeCage) — Portable bubblewrap sandbox that confines Claude Code to one project directory. *(★ 143, AGPL-3.0)*
- [Edera](https://edera.dev) — Kubernetes runtime that isolates pods in zones built on a microVM boundary.
- [FreeBSD Capsicum](https://man.freebsd.org/cgi/man.cgi?query=capsicum) — FreeBSD capability mode that drops a process's access to global namespaces.
- [FreeBSD Jails](https://docs.freebsd.org/en/books/handbook/jails/) — FreeBSD operating-system virtualization that isolates processes, files, and networking.
- [illumos Zones](https://illumos.org/man/8/zoneadm) — illumos and Solaris operating-system virtualization for isolated environments.
- [Landlock](https://docs.kernel.org/userspace-api/landlock.html) — Linux kernel feature that lets an unprivileged process restrict its own filesystem and network access.
- [macOS App Sandbox](https://developer.apple.com/documentation/security/app-sandbox) — Apple entitlement system that confines a Mac or iOS app to declared files and capabilities.
- [OpenBSD pledge](https://man.openbsd.org/pledge.2) — OpenBSD system call that limits a process to a named set of kernel operations.
- [OpenBSD unveil](https://man.openbsd.org/unveil.2) — OpenBSD system call that limits which filesystem paths a process can see.
- [seccomp](https://docs.kernel.org/userspace-api/seccomp_filter.html) — Linux syscall filter used by containers and code-execution jails.

## Dormant & Archived (Notable)

*Dead or archived projects kept for reference.*

- [Bytebot](https://www.bytebot.ai) — Desktop agent environment packaged as a container with a virtual display. *(★ 11.1k, Apache-2.0)* 📦 archived
- [Lucet](https://github.com/bytecodealliance/lucet) — Former Fastly native WebAssembly compiler and runtime, superseded by Wasmtime. *(★ 4k, Apache-2.0)* 📦 archived
- [Ignite](https://ignite.readthedocs.org) — Weaveworks tool that boots Firecracker microVMs from OCI images. *(★ 3.5k, Apache-2.0)* 📦 archived
- [Deno Deploy](https://deno.com/deploy) — Managed runtime for JavaScript isolates, including subhosting APIs. *(★ 367, MIT)* 📦 archived
- [Charliecloud](https://gitlab.com/charliecloud/main) — Unprivileged HPC container runtime based on user namespaces. *(★ 318, Apache-2.0)* 📦 archived
- [ERA](https://github.com/BinSquare/ERA) — Local krunvm-based sandbox with a container-like CLI. *(★ 305, Apache-2.0)* 📦 archived
- [Nabla containers](https://nabla-containers.github.io/) — OCI runtime that executes a unikernel image behind a thin monitor. *(★ 257, ISC)* 📦 archived
- [langchain-sandbox](https://github.com/langchain-ai/langchain-sandbox) — LangChain package that executes Python in a sandbox, including a Pyodide backend. *(★ 242)* 📦 archived
- [yolo-cage](https://github.com/borenstein/yolo-cage) — VM sandbox for coding agents that blocks secret exfiltration and self-merges. *(★ 109)* 📦 archived
- [Tenki Sandbox](https://tenki.cloud/products/sandbox) — Hardware-isolated Linux VMs for coding agents with warm start, snapshot, and fork. *(MIT)* 📦 archived

---

## Contributing

Pull requests welcome. Entries must link a canonical source (repository or homepage) and state what it does in one factual sentence. Suggest the section; we'll re-bucket if needed. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the maintainers have waived all copyright to this list.

*Generated from `data/agent-sandboxes.json` in the agentlist.io repo by `scripts/generate-awesome.py`. Entries are editorial records, not endorsements; stars/licenses are point-in-time snapshots.* Seeded by a Grok coverage sweep plus GitHub enrichment.
