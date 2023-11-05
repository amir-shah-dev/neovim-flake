# A simple neovim flake config

Heavily based on [Quoteme/neovim-flake](https://github.com/Quoteme/neovim-flake/tree/master)'s take on a simple neovim flake. The goal is to reduce the number of files and complexities, making more accessible for Nix newcomers.

## How to add plugins

Follow the comments laid out in `flake.nix` on how to build your plugin of choice. From there head to `init.vim` to add the plugin.

## Usage as a flake

[![FlakeHub](https://img.shields.io/endpoint?url=https://flakehub.com/f/amir-shah-dev/neovim-flake/badge)](https://flakehub.com/flake/amir-shah-dev/neovim-flake)

Add neovim-flake to your `flake.nix`:

```nix
{
  inputs.neovim-flake.url = "https://flakehub.com/f/amir-shah-dev/neovim-flake/*.tar.gz";

  outputs = { self, neovim-flake }: {
    # Use in your outputs
  };
}

```


