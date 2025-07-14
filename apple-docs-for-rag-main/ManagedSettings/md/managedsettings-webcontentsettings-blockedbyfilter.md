

- ManagedSettings
- WebContentSettings
-  blockedByFilter 

Type Property

# blockedByFilter

A description of the setting that controls which websites a user can access.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let blockedByFilter: SettingMetadata
```

## Discussion

The default value is WebContentSettings.FilterPolicy.none, which indicates that the system doesn’t block any websites.

## See Also

### Filtering Web Domains

var blockedByFilter: WebContentSettings.FilterPolicy?

The current policy for filtering websites.

enum FilterPolicy

The policies available for filtering web content based on specific web domains.

