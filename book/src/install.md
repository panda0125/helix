# Installation

We provide pre-built binaries on the [GitHub Releases page](https://github.com/helix-editor/helix/releases).

## OSX

TODO: brew tap

```
$ brew tap helix-editor/helix
$ brew install helix
```

## Linux

### NixOS

A [flake](https://nixos.wiki/wiki/Flakes) containing the package is available in
the project root. The flake can also be used to spin up a reproducible development
shell for working on Helix.

### Arch Linux

TODO: AUR

## Build from source

```
git clone --recurse-submodules --shallow-submodules -j8 https://github.com/helix-editor/helix
cd helix
cargo install --path helix-term
```

This will install the `hx` binary to `$HOME/.cargo/bin`.

Now copy the `runtime/` directory somewhere. Helix will by default look for the
runtime inside the same folder as the executable, but that can be overriden via
the `HELIX_RUNTIME` environment variable.