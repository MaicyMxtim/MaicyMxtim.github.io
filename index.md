# Maicy Maritim

Platform and machine learning infrastructure. I build the systems that run software and models in production: Kubernetes, GitOps, pipelines, observability, and the security controls around them.

Two projects, both built from nothing and documented in full, including what broke.

## Tamani Platform

A production platform running a venue discovery backend on Kubernetes. It serves a public API on AWS, routes every AI call through a governed gateway with caching and budget limits, runs two autonomous agents inside a safety layer, and enforces a signed supply chain.

| | |
|---|---|
| Live site | [platform.waypear.com](https://platform.waypear.com/) |
| Project page | [maicymxtim.github.io/tamani-platform](https://maicymxtim.github.io/tamani-platform/) |
| Source | [github.com/MaicyMxtim/tamani-platform](https://github.com/MaicyMxtim/tamani-platform) |

Built with AWS, OpenTofu, k3s, Argo CD, FastAPI, NATS, Redis, Prometheus, Grafana, Loki, Kyverno and cosign.

Availability was 100% with 95 ms at the 95th percentile in the measured window. A scaffold command takes a new service from nothing to serving live traffic in 195 seconds. Model tiering was measured to cut AI cost by about 57%.

## Akili Platform

An MLOps platform on Kubernetes. It validates incoming data, trains a model, decides whether the new model is good enough to replace the one in production, deploys it without downtime, and watches for the data changing underneath it. Container images and model files are both signed, and the cluster refuses to run anything unsigned.

| | |
|---|---|
| Project page | [maicymxtim.github.io/akili](https://maicymxtim.github.io/akili/) |
| Source | [github.com/MaicyMxtim/akili](https://github.com/MaicyMxtim/akili) |

Built with k3d, Argo CD, Argo Workflows, MinIO, MLflow, Feast, Redis, LightGBM, FastAPI, Argo Rollouts, Prometheus, Evidently and Kyverno.

The full retrain and deploy cycle runs with nobody involved. Killing a serving pod under load cost zero failed requests, and draining an entire node cost one request in ninety. A model whose signature has been altered will not load.

## Writing

Both projects include their failures. Between them there are seven incident reports covering memory exhaustion, an upstream release with a process leak, a service that reported itself healthy while every request failed, and a security control that locked the cluster out of its own recovery.

## Contact

| | |
|---|---|
| Email | [maicymaritim@gmail.com](mailto:maicymaritim@gmail.com) |
| GitHub | [github.com/MaicyMxtim](https://github.com/MaicyMxtim) |
