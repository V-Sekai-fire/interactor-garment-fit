# interactor-garment-fit

The garment fit stage as a godot-sandbox guest: an intersection-free retargeting solve with a signed-distance sampler emitted from Lean.

## What it is for

It fits a garment onto a body inside a sandbox guest, running the vendored retargeting solver one
phase per call, and the same sources build natively as the reference the guest is held to. The
signed-distance spline sampler the solver uses is written and checked in Lean, then emitted to
C++ and Slang under `kernels/`.

## Build

There is no standalone build. `transport-meshing-pen` builds the guest from a workspace checkout,
which places this repository beside the guest runtime and headers it links (RFD 2294).

## Licence

No licence is stated for this repository as a whole. The vendored solver is MIT; see
`vendor/cloth-fit/LICENSE`.
