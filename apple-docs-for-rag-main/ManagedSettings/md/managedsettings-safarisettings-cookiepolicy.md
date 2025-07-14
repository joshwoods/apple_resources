

- ManagedSettings
- SafariSettings
-  cookiePolicy 

Type Property

# cookiePolicy

The metadata for the setting that configures Safari’s policy for cookies.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let cookiePolicy: SettingMetadata
```

## Discussion

Use `cookiePolicy` to access the metadata for cookiePolicy. The default value is SafariSettings.CookiePolicy.always.

## See Also

### Specifying a Cookie Policy

var cookiePolicy: SafariSettings.CookiePolicy?

Defines the conditions under which Safari accepts cookies.

enum CookiePolicy

The conditions under which Safari accepts cookies.

