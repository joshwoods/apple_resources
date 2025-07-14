

- ManagedSettings
- ShieldSettings
-  applications 

Type Property

# applications

The metadata for the configuration that specifies apps for the system to cover with a shielding view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let applications: SettingMetadata>
```

## Discussion

The default value is an empty set.

## See Also

### Blocking Apps and Websites

var applications: Set&lt;ApplicationToken>?

Applications for the system to cover with a shielding view.

var webDomains: Set&lt;WebDomainToken>?

Websites for the system to cover with a shielding view.

static let webDomains: SettingMetadata&lt;Set&lt;WebDomainToken>>

The metadata for the configuration that specifies websites for the system to shield.

