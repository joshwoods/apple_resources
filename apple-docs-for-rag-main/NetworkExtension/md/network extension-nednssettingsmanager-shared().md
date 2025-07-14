

- Network Extension
- NEDNSSettingsManager
-  shared() 

Type Method

# shared()

Access the single instance of a DNS settings manager.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class func shared() -> NEDNSSettingsManager
```

## Return Value

The DNS settings manager instance for the calling application.

## See Also

### Managing DNS configurations

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load your DNS settings configuration from the system networking preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Save your DNS settings configuration to the system networking preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Remove your DNS settings configuration from the system networking preferences.

