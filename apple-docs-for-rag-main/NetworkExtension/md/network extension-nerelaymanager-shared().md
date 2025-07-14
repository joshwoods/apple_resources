

- Network Extension
- NERelayManager
-  shared() 

Type Method

# shared()

Access the single instance of a network relay manager.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class func shared() -> NERelayManager
```

## Return Value

The network relay manager instance for the calling application.

## See Also

### Managing relay configurations

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load your relay configuration from the system networking preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Save your relay configuration to the system networking preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Remove your relay configuration from the system networking preferences.

