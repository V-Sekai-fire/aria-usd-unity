# AriaUsdUnity

Unity ↔ USD conversion package for Elixir.

## Overview

This package provides bidirectional conversion between Unity packages and USD format. It depends on `aria_usd` for core USD operations.

## Installation

Add `aria_usd_unity` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [
    {:aria_usd_unity, path: "../apps/aria_usd_unity"},
    {:aria_usd, git: "https://github.com/V-Sekai-fire/aria-usd.git"}
  ]
end
```

## Usage

```elixir
# Convert USD to Unity package
AriaUsdUnity.usd_to_unity_package("model.usd", "output.unitypackage")

# Convert Unity assets to USD
AriaUsdUnity.convert_unity_to_usd("asset.unity", "output.usd")

# Import Unity package
AriaUsdUnity.import_unity_package("package.unitypackage", "/path/to/extract")
```

## Requirements

- Elixir ~> 1.18
- `aria_usd` package
- USD Python bindings (pxr)

## License

MIT

