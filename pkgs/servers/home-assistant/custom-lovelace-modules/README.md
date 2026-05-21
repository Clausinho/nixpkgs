# Packaging guidelines

## Entrypoint

Every lovelace module has an entrypoint in the form of a `.js` file. By
default the nixos module will try to load `${pname}.js` when a module is
configured.

The entrypoint used can be overridden in `passthru` like this:

```nix
{ passthru.entrypoint = "demo-card-bundle.js"; }
```

<!-- PARA-WIKI-LINKS:START -->
## Wiki Links
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/advanced-camera-card/README|advanced camera card]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/apexcharts-card/README|apexcharts card]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/atomic-calendar-revive/README|atomic calendar revive]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/auto-entities/README|auto entities]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/battery-state-card/README|battery state card]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/bubble-card/README|bubble card]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/button-card/README|button card]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/card-mod/README|card mod]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/clock-weather-card/README|clock weather card]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/custom-sidebar/README|custom sidebar]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/decluttering-card/README|decluttering card]]
- [[02_Areas/60_Infrastructure/60.01_nix-config/nixpkgs/pkgs/servers/home-assistant/custom-lovelace-modules/flower-card/README|flower card]]
<!-- PARA-WIKI-LINKS:END -->
