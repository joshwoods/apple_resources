

- Network Extension
- NEAppPushManager
-  isEnabled 

Instance Property

# isEnabled

A property you use to toggle enabling the configuration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

The framework sets this value to NO when your app saves a configuration that overlaps with this configuration. This overlap occurs when a new NEAppPushManager saves a configuration with a matchSSIDs list that contains an SSID which is also a member of this manager’s SSID list.

## See Also

### Inspecting manager properties

var isActive: Bool

A Boolean value that indicates whether a configuration is in use.

var localizedDescription: String?

A string that contains the localized description of the app push manager.

