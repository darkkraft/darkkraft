<h1 align="center">Infrastructure Engineer &nbsp;·&nbsp; Architect</h1>

<p align="center">
  <em>Architecture &nbsp;·&nbsp; scalable infrastructure &nbsp;·&nbsp; low latency</em>
</p>

<p align="center">
  <code>big tech</code> <code>HFT</code> <code>PSP</code> <code>big data</code> <code>fintech</code> <code>blockchain</code>
</p>

<p align="center">16+ years of infrastructure engineering.</p>

<br>

**Security** &nbsp;— &nbsp;confidential computing with TDX, SGX, AMD SEV and AWS Nitro, MPC, SOC 2

**Low latency** &nbsp;— &nbsp;Solarflare, kernel bypass, kernel patching, NIC firmware and IRQ tuning, Arista fabrics

**Cloud and bare metal** &nbsp;— &nbsp;AWS, GCP, Azure, OVH, and hardware I provision myself: custom KVM and libvirt layers, immutable images with mkosi and dm-verity, measured boot, Talos

**Scale** &nbsp;— &nbsp;past 10,000 nodes across regions, on cloud, on-prem and hybrid

**Observability** &nbsp;— &nbsp;Prometheus, Grafana, Loki, Tempo, Thanos, Vector, custom exporters

**AI** &nbsp;— &nbsp;I plan, build, verify, test, security-scan and maintain with AI tooling in the loop. I also build *for* AI: agents and agent tooling, MCP servers, LLM gateways, agent memory, and the inference infrastructure underneath

<br>

## Selected work

<table>
<tr><td width="50%" valign="top">

#### [gpuscale](https://github.com/munhq/gpuscale)
<sub><code>Go</code> <code>Kubernetes</code> <code>Apache-2.0</code></sub>

A Kubernetes controller that provisions GPU capacity from seven providers, selects the cheapest offer that meets the requirements, serves vLLM on it, and scales to zero when demand stops.

<sub>GPU prices differ by multiples between providers. Karpenter supports AWS and Azure only, and Cluster Autoscaler requires node groups defined in advance. Neither can buy a spot GPU from a marketplace.</sub>

</td><td width="50%" valign="top">

#### [kubernetes_gpu](https://github.com/munhq/kubernetes_gpu)
<sub><code>Go</code> <code>Ansible</code> <code>Apache-2.0</code></sub>

Three Ansible playbooks deploy an LLM inference API on your own GPUs — batch endpoint, dashboard, per-GPU DCGM metrics, autoscaling, GitOps, WireGuard mesh across clouds. One variable selects Ray or gpuscale for capacity.

<sub>Integrates K3s, KubeRay, vLLM, ArgoCD, DCGM, KEDA and WireGuard into one deployable platform.</sub>

</td></tr>
<tr><td width="50%" valign="top">

#### [cloud-tools](https://github.com/munhq/cloud-tools)
<sub><code>Rust</code> <code>MCP</code> <code>Apache-2.0</code></sub>

Cost, inventory and waste analysis across AWS, GCP, Cloudflare and OVH. Finds what is idle, oversized, previous-generation or unattached by combining inventory with utilisation, not one dimension.

<sub>Runs as an MCP server and an HTTP API, so an AI agent can query spend and waste directly.</sub>

</td><td width="50%" valign="top">

#### [codeindex](https://github.com/munhq/codeindex)
<sub><code>Zig</code> <code>MCP</code> <code>MIT</code></sub>

Structural code intelligence for AI agents — tree-sitter across 40+ languages, trigram and inverted indexes, a dependency graph, behind 19 MCP tools.

<sub>Answers structural questions — definitions, callers, dependencies, blast radius — in a few hundred tokens instead of whole files.</sub>

</td></tr>
<tr><td colspan="2" valign="top">

#### [platform-k3d](https://github.com/darkkraft/platform-k3d)
<sub><code>OpenTofu</code> <code>Terragrunt</code> <code>Rust</code> <code>MIT</code></sub>

A reference GitOps platform: cluster and services as reusable modules, Argo CD app-of-apps per environment, Rust microservices on Axum and sqlx, CI pipelines, and scripts that bring the whole thing up and tear it down again.

<sub>Brings up dev, staging and prod as separate k3d clusters from one script, with CI, secrets and observability included.</sub>

</td></tr>
</table>

