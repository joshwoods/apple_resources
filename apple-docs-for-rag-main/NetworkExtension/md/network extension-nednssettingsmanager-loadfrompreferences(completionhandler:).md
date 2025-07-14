

- Network Extension
- NEDNSSettingsManager
-  loadFromPreferences(completionHandler:) 

Instance Method

# loadFromPreferences(completionHandler:)

Load your DNS settings configuration from the system networking preferences.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func loadFromPreferences(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func loadFromPreferences() async throws
```

## Parameters 

`completionHandler`  

A block that takes an NSError object. This block runs on your application’s main thread after the load operation is complete. If an error occurs while loading the configuration, the block returns an `NSError` object.

## Discussion

You must call this method at least once before calling saveToPreferences(completionHandler:) for the first time after your app launches.

## See Also

### Managing DNS configurations

class func shared() -> NEDNSSettingsManager

Access the single instance of a DNS settings manager.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Save your DNS settings configuration to the system networking preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Remove your DNS settings configuration from the system networking preferences.

