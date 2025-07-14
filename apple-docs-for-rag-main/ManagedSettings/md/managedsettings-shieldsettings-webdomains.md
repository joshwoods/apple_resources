

- ManagedSettings
- ShieldSettings
-  webDomains 

Type Property

# webDomains

The metadata for the configuration that specifies websites for the system to shield.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let webDomains: SettingMetadata>
```

## Discussion

Use `webDomains` to access the metadata for webDomains. The default value is an empty set.

## See Also

### Blocking Apps and Websites

var applications: Set&lt;ApplicationToken>?

Applications for the system to cover with a shielding view.

static let applications: SettingMetadata&lt;Set&lt;ApplicationToken>>

The metadata for the configuration that specifies apps for the system to cover with a shielding view.

var webDomains: Set&lt;WebDomainToken>?

Websites for the system to cover with a shielding view.

