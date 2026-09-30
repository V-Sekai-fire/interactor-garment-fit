# interactor-garment-fit

The fit stage as a godot-sandbox guest: cloth-fit's PolyFEM garment solve with the Lean SDF sampler.

Split out of `interactor-dress-on` at `310b52e` with its history (`git subtree`). It sits at `3-interactor/garment-fit` in the goal manifest (`contract-manifest-taskweft`), and finds the repositories it builds against as sibling checkouts at their manifest paths. `transport-meshing-pen` builds the guest ELFs (`build.sh`, `tools/build.exs`).
