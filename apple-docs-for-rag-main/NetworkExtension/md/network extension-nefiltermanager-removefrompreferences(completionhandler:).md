

- Network Extension
- NEFilterManager
-  removeFromPreferences(completionHandler:) 

Instance Method

# removeFromPreferences(completionHandler:)

Remove the filter configuration from the Network Extension preferences.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func removeFromPreferences(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func removeFromPreferences() async throws
```

## Parameters 

`completionHandler`  

A block that takes an NSError object. This block will be executed on the caller’s main thread after the removal operation is complete. If the configuration does not exist in the Network Extension preferences or an error occurs while removing it, the error parameter will be set to an `NSError` object containing details about the error. See `NEFilterManagerError` for a list of possible errors. If the configuration is removed successfully the error parameter will be set to nil.

## Discussion

After the configuration is removed from the preferences the `NEFilterManager` object will still contain the configuration parameters. Calling `loadFromPreferencesWithCompletionHandler:` will clear out the configuration parameters from the `NEFilterManager` object.

## See Also

### Managing the filter configuration

class func shared() -> NEFilterManager

Access the single instance of `NEFilterManager`.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load the filter configuration from the Network Extension preferences.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Save the filter configuration in the Network Extension preferences.

