<h1 align="center">Infrastructure Engineer &nbsp;·&nbsp; Architect</h1>

<p align="center">
  <em>Architecture &nbsp;·&nbsp; scalable infrastructure &nbsp;·&nbsp; low latency</em>
</p>

<p align="center">
  <code>big tech</code> <code>HFT</code> <code>PSP</code> <code>big data</code> <code>fintech</code> <code>blockchain</code>
</p>

<p align="center">16+ years. Builder. I start new things to challenge myself.</p>

<br>

**Security** &nbsp;— &nbsp;confidential computing with TDX, SGX, AMD SEV and AWS Nitro, MPC, SOC 2

**Low latency** &nbsp;— &nbsp;Solarflare, kernel bypass, kernel patching, NIC firmware and IRQ tuning, Arista fabrics

**Cloud or bare metal, same problem** &nbsp;— &nbsp;AWS, GCP, Azure, OVH, or hardware I provision myself: custom KVM and libvirt layers, immutable images with mkosi and dm-verity, measured boot, Talos. The platform is a detail; I build whatever the project needs

**Scale** &nbsp;— &nbsp;past 10,000 nodes across regions, worldwide, on cloud, on-prem and hybrid

**Observability everywhere**

**AI** &nbsp;— &nbsp;I used to build manually. Now I do everything with AI: planning, verifying, re-verifying, validating, testing, security scanning and maintaining. AI is everywhere and I am at the centre of it, supervising and sometimes managing it. I build *for* AI too — agents and agent tooling, MCP servers, LLM gateways, agent memory, and the inference infrastructure underneath

<br>

## Selected work

<table>
<tr><td width="50%" valign="top">

#### [gpuscale](https://github.com/munhq/gpuscale)
<sub><code>Go</code> <code>Kubernetes</code> <code>Apache-2.0</code></sub>

Run LLM inference on the cheapest GPU available anywhere, and stop paying for it when nobody is asking. A controller that shops seven providers, buys the cheapest instance that fits, serves vLLM on it, and scales to zero.

<sub>GPU prices differ by multiples between providers and no open-source autoscaler can act on it. Karpenter is AWS and Azure only. Cluster Autoscaler needs node groups up front. Neither can buy a spot GPU from a marketplace.</sub>

</td><td width="50%" valign="top">

#### [kubernetes_gpu](https://github.com/munhq/kubernetes_gpu)
<sub><code>Go</code> <code>Ansible</code> <code>Apache-2.0</code></sub>

Three playbooks and you have an LLM inference API on your own GPUs — batch endpoint, dashboard, per-GPU DCGM metrics, autoscaling, GitOps, WireGuard mesh across clouds. One variable picks Ray or gpuscale for capacity.

<sub>Standing this up means gluing a dozen components that each assume the others do not exist. This is the assembled thing, wiring done.</sub>

</td></tr>
<tr><td width="50%" valign="top">

#### [cloud-tools](https://github.com/munhq/cloud-tools)
<sub><code>Rust</code> <code>MCP</code> <code>Apache-2.0</code></sub>

Cost, inventory and waste analysis across AWS, GCP, Cloudflare and OVH. Finds what is idle, oversized, previous-generation or unattached by combining inventory with utilisation, not one dimension.

<sub>Cost tools tell you what you spent. They rarely tell you what you are wasting, and never across four providers at once.</sub>

</td><td width="50%" valign="top">

#### [codeindex](https://github.com/munhq/codeindex)
<sub><code>Zig</code> <code>MCP</code> <code>MIT</code></sub>

Structural code intelligence for AI agents — tree-sitter across 40+ languages, trigram and inverted indexes, a dependency graph, behind 19 MCP tools.

<sub>Agents burn their context window reading whole files to answer questions an index answers in a line.</sub>

</td></tr>
<tr><td colspan="2" valign="top">

#### [platform-k3d](https://github.com/darkkraft/platform-k3d)
<sub><code>OpenTofu</code> <code>Terragrunt</code> <code>Rust</code> <code>MIT</code></sub>

A reference GitOps platform: cluster and services as reusable modules, Argo CD app-of-apps per environment, Rust microservices on Axum and sqlx, CI pipelines, and scripts that bring the whole thing up and tear it down again.

<sub>The worked example — how the pieces fit when someone has actually assembled them, rather than a diagram of how they might.</sub>

</td></tr>
</table>

<br>

<p align="center">Work is never done. The factory must grow.</p>
