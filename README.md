# Rebel Build Action

Github Action for building Rebel Engine.

This Action provides a standardised way for building Rebel Engine and Rebel Editor. It uses [`actions/upload-artifact@v4`](https://github.com/actions/upload-artifact) to allow the executable or library that is built to be downloaded as an artifact.

## Usage

### Inputs
```
- uses: RebelToolbox/RebelBuildAction@v4
  with:
    # Name of the artifact to be uploaded
    artifact:

    # SCons build options
    build-options:

    # Build Rebel with Mono module
    # Type: boolean
    # Default: false
    include-mono:

    # Use a build cache to make subsequent builds faster
    # Type: boolean
    # Default: true
    use-build-cache:
```

### Outputs
| Name | Description |
| - | - |
| `build-filename` | The filename of the executable or library created by building Rebel with the specified build options. |
