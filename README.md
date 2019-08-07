# Rust Kubernetes Controller

This is an example of how easy it is to write Kubernetes controllers (operators) for Custom Resource Definitions (CRDs) in Rust. No more special generation programs, verbose configurations, and massive boilerplate... just quick and easy Kubernetes controllers.

This repository has a CRD, a CRD instance, and a simple `informer`-style controller. You can build and run the code by fetching this repo and then running `cargo run`.

The entire code is in `src/main.rs`.

## Instructions

- Make sure you have the latest Rust installed
- Make sure you have `kubectl` installed and configured to point to a cluster
- Download this code
- Run `kubectl create -f docs/crd.yaml`
- Run `cargo run` and keep it running
- Wait a moment for it to start
- Run `kubectl create -f docs/book.yaml`
- Observe the output in the `cargo run`

To stop `cargo run`, use `CTRL-C`.

> This will run the controller locally, rather than in-cluster.