

- Network Extension
- NERelayManager
-  removeFromPreferences(completionHandler:) 

Instance Method

# removeFromPreferences(completionHandler:)

Remove your relay configuration from the system networking preferences.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

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

After you remove your configuration, the NERelayManager object still contains the configuration parameters. Calling loadFromPreferences(completionHandler:) clears out the configuration parameters from the NERelayManager object.

## See Also

### Managing relay configurations

class func shared() -> NERelayManager

Access the single instance of a network relay manager.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load your relay configuration from the system networking preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Save your relay configuration to the system networking preferences.

