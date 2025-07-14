

- Network Extension
- NEAppPushManager
-  removeFromPreferences(completionHandler:) 

Instance Method

# removeFromPreferences(completionHandler:)

Removes the manager’s configuration from the persistent store.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func removeFromPreferences(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func removeFromPreferences() async throws
```

## Parameters 

`completionHandler`  

A completion block that the framework calls after it removes the configuration. If removal failed, the `error` parameter indicates the reason for the failure; otherwise, this parameter is `nil`.

## See Also

### Persisting manager settings

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Loads the manager’s saved configuration from the persistent store.

class func loadAllFromPreferences(completionHandler: ([NEAppPushManager]?, (any Error)?) -> Void)

Loads all saved manager configurations asynchronously.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Saves the manager’s configuration in the persistent store.

