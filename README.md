# Hemant Kumar Singh

I build developer tools for webhooks and APIs. TypeScript · Node · React · Go.

### [HookLens](https://github.com/merak-max/hooklens) · Developer tools

Self-hosted webhook inspector with live capture, HMAC-SHA256 verification,
and guarded replay to configured hosts. Built with TypeScript, Node, and React.

Generated capture endpoints, live updates over Server-Sent Events, searchable
delivery history, API and browser tests, and a Docker setup.

[Quickstart](https://github.com/merak-max/hooklens#local-development) ·
[Architecture](https://github.com/merak-max/hooklens#architecture) ·
[Security boundaries](https://github.com/merak-max/hooklens/blob/main/SECURITY.md)

### [Auction Engine](https://github.com/merak-max/auction-engine) · Backend systems

Go service for single-slot second-price and multi-slot GSP auctions, with
daily budget pacing, atomic reservations, and auction-ID replay protection.
PostgreSQL shares the spend ledger across server instances.

**Published benchmark: 5.51 ms p99** across 50,000 three-slot requests at eight
concurrent clients, with zero errors or no-fills. Measured September 26, 2026,
on a Linux/ARM64 host with eight logical CPUs and synchronous PostgreSQL
commits. Client and server ran on the same host; this closed-loop result is
not a WAN or production latency guarantee.

[Reproduce the benchmark](https://github.com/merak-max/auction-engine/tree/main/benchmarks) ·
[Raw result](https://github.com/merak-max/auction-engine/blob/7550473f9f202938f6350659a273d6217984b36d/benchmarks/postgres-gsp-single.json) ·
[Architecture and tradeoffs](https://github.com/merak-max/auction-engine#architecture)

### Also built

- [Blue Carbon Registry](https://github.com/merak-max/blue-carbon-registry): a prototype for carbon-project verification workflows and credit accounting.
- [Developer portfolio](https://github.com/merak-max/hemant-portfolio): selected projects, with a [live site](https://hemant-portfolio-hazel.vercel.app).
