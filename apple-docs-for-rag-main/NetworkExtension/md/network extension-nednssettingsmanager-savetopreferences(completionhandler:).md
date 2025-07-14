

- Network Extension
- NEDNSSettingsManager
-  saveToPreferences(completionHandler:) 

Instance Method

# saveToPreferences(completionHandler:)

Save your DNS settings configuration to the system networking preferences.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func saveToPreferences(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func saveToPreferences() async throws
```

## Parameters 

`completionHandler`  

An optional block that takes an NSError object. If specified, this block runs on your application’s main thread after the save operation completes. If an error occurs while saving the configuration, the block returns an `NSError` object.

## Discussion

You must call loadFromPreferences(completionHandler:) at least once before calling this method the first time after your app launches.

## See Also

### Managing DNS configurations

class func shared() -> NEDNSSettingsManager

Access the single instance of a DNS settings manager.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load your DNS settings configuration from the system networking preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Remove your DNS settings configuration from the system networking preferences.

