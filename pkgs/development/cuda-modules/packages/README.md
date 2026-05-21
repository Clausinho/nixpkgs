# packages

Packages which are not created by the redistributable builder.

## Conventions

- All new packages should include the following lines as part of their arguments to `stdenv.mkDerivation`:

  ```nix
  finalAttrs: {
    __structuredAttrs = true;
    strictDeps = true;

    # NOTE: Depends on the CUDA package set, so use cudaNamePrefix.
    name = "${cudaNamePrefix}-${finalAttrs.pname}-${finalAttrs.version}";
  }
  ```

  If the package does not require elements of the package set, then the `cudaNamePrefix` must be omitted: changing the name of a derivation yields a different hash and store path, so we would end up with multiple different store paths with the same content.

<!-- PARA-WIKI-LINKS:START -->
## Wiki Links
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/cuda-modules/packages/autoAddCudaCompatRunpath/README|autoAddCudaCompatRunpath]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/cuda-modules/packages/cudnn-frontend/README|cudnn frontend]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/cuda-modules/packages/markForCudatoolkitRootHook/README|markForCudatoolkitRootHook]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/cuda-modules/packages/removeStubsFromRunpathHook/README|removeStubsFromRunpathHook]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/cuda-modules/packages/saxpy/README|saxpy]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/cuda-modules/packages/setupCudaHook/README|setupCudaHook]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/cuda-modules/packages/tensorrt-samples/README|tensorrt samples]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/cuda-modules/packages/tests/README|tests]]
<!-- PARA-WIKI-LINKS:END -->
