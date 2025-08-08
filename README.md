# setup-python-embedded

Download and extract Python embedded into current working directory.

- - -

## Usage

```yaml
- name: Setup Python Embedded for Windows
  uses: BHznJNs/setup-python-embedded@release-1
```

## Parameters

### Inputs

| Name             | Required | Default | Description |
|------------------|----------|---------|-------------|
| `python-version` | ✅        | `3.11.9`| Target Python embedded version to download (e.g. `3.12.7`). |
| `arch`           | ❌        | `amd64` | Target Windows architecture. Must be one of: `amd64`, `win32`, `arm64`. |

### Outputs

| Name                   | Description |
|------------------------|-------------|
| `python-embedded-path` | path to the extracted Python embedded directory. <br>Use this folder with `python.exe` directly to downstream steps. |
