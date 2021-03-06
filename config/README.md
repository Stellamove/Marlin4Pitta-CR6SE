# CR-6 community configuration examples

You can find various example configurations in the sub-directories.

The following examples are available: 

**For the CR-6 SE:**

- [With v4.5.3 motherboard](./cr6-se-v4.5.3-mb)

## Helper scripts

There are some helper scripts. You need Powershell Core (`pwsh`) to run them.

### Generating configuration examples

To generate or update a configuration example, do the modifications and then run:

    scripts/Generate-ConfigExample.ps1 -Name MyExampleName

### Applying configuration examples

To apply a configuration example, just copy the `Configuration*` files from the example directory to the "Marlin" directory.

### Maintenance

To refresh configuration examples (repository maintainers):

    scripts/Update-ConfigExamples.ps1

This script essentially runs an update on all configuration examples based on the changes of the current configuration (diff).

### Run builds

To run builds for all examples (repository maintainers):

    scripts/Run-ExampleConfigBuilds.ps1 -TouchscreenRepositoryPath [path to cr6 touch screen repository]

This script is meant to be executed in the VSCode console and in preperation for firmware release.

#### How it works

The base configuration for this repository is based on the most common hardware configuration: The Creality CR-6 SE with v4.5.2 motherboard. All other configurations are derived from that configuration. Using diff files the original configuration can be amended, then built.