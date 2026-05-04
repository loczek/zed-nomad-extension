# Overview

A [Zed](https://zed.dev) extension for the [nomad-ls](https://github.com/loczek/nomad-ls) language server.

## Configure file associations

The only defaults suffixes are `.nomad` and `.nomad.hcl` that match to `Nomad Job`, other languages need to be configured to work e.g.

```jsonc
// .zed/settings.json
{
  "file_types": {
    "Nomad ACL": ["**/*.nomad.acl"],
    "Nomad Agent": ["**/*.nomad.client", "**/*.nomad.server"],
    "Nomad CSI Volume": ["**/*.nomad.csi"],
    "Nomad Dynamic Host Volume": ["**/*.nomad.dyn"],
    "Nomad Job": ["**/*.nomad"],
    "Nomad Namespace": ["**/*.nomad.ns"],
    "Nomad Node Pool": ["**/*.nomad.np"],
    "Nomad Resource Quota": ["**/*.nomad.rq"],
    "Nomad Variable": ["**/*.nomad.var"]
  }
}
```

> [!Note]
> You may need to restart your editor for the changes to take effect

## Build and install in Zed

You can install this as a dev extension directly in Zed:

1. Open Zed's command palette (`Cmd+Shift+P`)
1. Run `zed: install dev extension`
1. Navigate to and select the `zed-nomad-extension` directory

Zed will automatically build and load the extension from the source directory.
