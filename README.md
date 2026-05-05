# Sytone's Scoop Bucket

[![CI](https://github.com/sytone/sytones-scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/sytone/sytones-scoop-bucket/actions/workflows/ci.yml)
[![Excavator](https://github.com/sytone/sytones-scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/sytone/sytones-scoop-bucket/actions/workflows/excavator.yml)

A bucket for [Scoop](https://scoop.sh) containing apps I use.

## Usage

```pwsh
scoop bucket add sytone https://github.com/sytone/sytones-scoop-bucket
```

Then install any app:

```pwsh
scoop install sytone/<app-name>
```

## Apps

| App | Description |
|-----|-------------|
| [asmspy](https://github.com/mikehadlow/AsmSpy) | A simple command line tool to view assembly references |
| [azcopy](https://docs.microsoft.com/en-us/azure/storage/common/storage-use-azcopy-v10) | Command-line utility for copying data to/from Azure Storage |
| [czkawkagui](https://github.com/qarmin/czkawka) | Tool to find duplicates, similar images and music |
| [dotnet-sdk-helper](https://github.com/sytone/dotnet-sdk-cli) | Helps manage .NET SDK versions from the command line |
| [flow-launcher](https://github.com/Flow-Launcher/Flow.Launcher) | Dedicated workflow launcher — searches, integrates and expands on functionalities |
| [git-credential-manager-core](https://github.com/microsoft/Git-Credential-Manager-Core) | Git Credential Manager Core |
| [LM-Studio](https://lmstudio.ai) | Run LLMs on your laptop, entirely offline |
| [powershell-simplesettings](https://github.com/sytone/simplesettings) | Simple setting solution for PowerShell |
| [psnet](https://github.com/psmux/psnet) | Real-time TUI network monitor for Windows |
| [pstop](https://github.com/psmux/pstop) | htop for Windows — beautiful, fast TUI system monitor |
| [rememberthemilk](https://www.rememberthemilk.com) | The smart to-do app for busy people |
| [vs2022-enterprise](https://www.visualstudio.com/) | Visual Studio 2022 Enterprise |
| [wox-prerelease](http://www.wox.one) | A full-featured launcher for accessing programs and web contents |

## How It Works

This bucket follows the [ScoopInstaller/BucketTemplate](https://github.com/ScoopInstaller/BucketTemplate) structure:

- **Manifests** are stored in the `bucket/` directory
- **Excavator** (GitHub Actions) automatically checks for and applies version updates every 4 hours
- **CI tests** validate all manifests on every push and pull request
- **bin/** contains helper scripts for local development (`checkver`, `checkhashes`, etc.)
