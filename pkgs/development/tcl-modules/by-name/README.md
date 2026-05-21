# Name-based Tcl package directories

The structure of this directory is identical to the one described in
[/pkgs/by-name/README.md](../../../by-name/README.md).
The only difference is the scope:

```nix
{
  lib,
  # You can get tclPackages attributes directly
  mkTclDerivation,
  tcllib,
}:

mkTclDerivation {
  # ...
}
```

<!-- PARA-WIKI-LINKS:START -->
## Wiki Links
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/bw/README|bw]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/ex/README|ex]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/in/README|in]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/it/README|it]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/le/README|le]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/mu/README|mu]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/pd/README|pd]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/rl/README|rl]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/ru/README|ru]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/tc/README|tc]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/td/README|td]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/development/tcl-modules/by-name/ti/README|ti]]
<!-- PARA-WIKI-LINKS:END -->
