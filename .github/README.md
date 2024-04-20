# My Personal Wiki

Kenrendell's [personal wiki](https://kenrendell.github.io/kenrendell-wiki/) (based on [emanote](https://emanote.srid.ca/)).

## Running using Nix

To start the Emanote live server using Nix:

```sh
nix run
```

To update Emanote version in flake.nix:

```sh
nix flake lock --update-input emanote
```

To build the static website via Nix:

```sh
nix build -o ./result
# Then test it:
nix run nixpkgs#nodePackages.live-server -- ./result
```
