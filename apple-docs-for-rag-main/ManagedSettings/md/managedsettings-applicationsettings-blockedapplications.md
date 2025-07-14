

- ManagedSettings
- ApplicationSettings
-  blockedApplications 

Type Property

# blockedApplications

A description of the setting that controls which apps a user can launch on their device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let blockedApplications: SettingMetadata>
```

## Discussion

Use `blockedApplications` to access the metadata for blockedApplications. The default value is an empty set.

## See Also

### Blocking Applications

var blockedApplications: Set&lt;Application>?

A set of applications for the system to block.

