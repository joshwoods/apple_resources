

- Network Extension
- NEFilterManager
-  saveToPreferences(completionHandler:) 

Instance Method

# saveToPreferences(completionHandler:)

Save the filter configuration in the Network Extension preferences.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func saveToPreferences(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func saveToPreferences() async throws
```

## Parameters 

`completionHandler`  

A block that takes an NSError object. This block will be executed on the caller’s main thread after the save operation is complete. If the configuration could not be saved to the preferences, the error parameter will be set to an `NSError` object containing details about the error. See `NEFilterManagerError` for a list of possible errors. If the configuration is saved successfully then the error parameter will be set to nil.

## Discussion

You must call `loadFromPreferencesWithCompletionHandler:` at least once before calling this method the first time after your app launches.

## See Also

### Managing the filter configuration

class func shared() -> NEFilterManager

Access the single instance of `NEFilterManager`.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load the filter configuration from the Network Extension preferences.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Remove the filter configuration from the Network Extension preferences.

