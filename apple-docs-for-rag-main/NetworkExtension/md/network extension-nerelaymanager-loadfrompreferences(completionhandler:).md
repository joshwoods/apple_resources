

- Network Extension
- NERelayManager
-  loadFromPreferences(completionHandler:) 

Instance Method

# loadFromPreferences(completionHandler:)

Load your relay configuration from the system networking preferences.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

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

### Managing relay configurations

class func shared() -> NERelayManager

Access the single instance of a network relay manager.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Save your relay configuration to the system networking preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Remove your relay configuration from the system networking preferences.

