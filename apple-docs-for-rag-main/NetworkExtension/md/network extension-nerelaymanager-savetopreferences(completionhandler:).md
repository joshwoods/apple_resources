

- Network Extension
- NERelayManager
-  saveToPreferences(completionHandler:) 

Instance Method

# saveToPreferences(completionHandler:)

Save your relay configuration to the system networking preferences.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

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

### Managing relay configurations

class func shared() -> NERelayManager

Access the single instance of a network relay manager.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load your relay configuration from the system networking preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Remove your relay configuration from the system networking preferences.

