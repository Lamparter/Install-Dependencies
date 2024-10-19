# 📊 Install Dependencies Action

#### A simple action to install dependencies for building a WinAppSdk app.

---

## 🔤 Inputs

### `target-platform`

**Optional** The platform to install dependencies for. Default is `all`.

### `dotnet-version`

**Optional** The .NET SDK version to install. Default is `8.0.x`.

### `sdk-version`

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
      - name: Install WinAppSDK workload
        uses: Lamparter/Install-Dependencies@v1.2.1
        with:
          target-platform: 'all'
          dotnet-version: '8.0.x'
          sdk-version: '19041'
```
