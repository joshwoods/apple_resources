

- Network Extension
- NEDNSSettingsManager
-  removeFromPreferences(completionHandler:) 

Instance Method

# removeFromPreferences(completionHandler:)

Remove your DNS settings configuration from the system networking preferences.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func removeFromPreferences(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func removeFromPreferences() async throws
```

## Parameters 

`completionHandler`  

An optional block that takes an NSError object. If specified, this block runs on your application’s main thread after your configuration is removed. If an error occurs while removing the configuration, the block returns an `NSError` object.

## Discussion

After you remove your configuration, the `NEDNSSettingsManager` object still contains the configuration parameters. Calling loadFromPreferences(completionHandler:) clears out the configuration parameters from the `NEDNSSettingsManager` object.

## See Also

### Managing DNS configurations

class func shared() -> NEDNSSettingsManager

Access the single instance of a DNS settings manager.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load your DNS settings configuration from the system networking preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Save your DNS settings configuration to the system networking preferences.

