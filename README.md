# 📊 Install Dependencies Action

#### A simple action to install dependencies for building an Uno Platform app.

---

## 🔤 Inputs

### `target-platform`

**Optional** The platform to install dependencies for. Default is `all`.

### `dotnet-version`

**Optional** The .NET SDK version to install. Default is `8.0.x`.

### `sdkVersion`

**Optional** The version of the Windows SDK to install. Default is `19041`.

## ⚡  Example Usage

```yaml
name: Example Workflow
on: [push]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Install Uno Workload
        uses: Lamparter/Install-UnoDependencies@v1.1.0
        with:
          target-platform: 'all'
          dotnet-version: '8.0.x'
          sdkVersion: '19041'
```
