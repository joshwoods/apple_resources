

- Device Management
- InstallEnterpriseApplicationCommand
- InstallEnterpriseApplicationCommand.Command
-  InstallEnterpriseApplicationCommand.Command.Manifest 

Device Management Command

# InstallEnterpriseApplicationCommand.Command.Manifest

A dictionary that contains a manifest.

macOS 10.13.6+Device Assignment ServicesVPP License Management

``` source
object InstallEnterpriseApplicationCommand.Command.Manifest
```

## Properties

`ANY`

`any`

A manifest, which is backward-compatible with the manifest for the `InstallApplication` command; however, it also allows you to specify `sha256s` and `sha256-size` for SHA-256 hashes.

## See Also

### Commands

object InstallEnterpriseApplicationCommand.Command.Configuration

A dictionary that contains the configuration to install an enterprise app.

object ManifestURL

The URL to the app manifest.

object ManifestURL.ItemsItem.Metadata

