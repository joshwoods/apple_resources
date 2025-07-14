

- Network Extension
- NEAppPushManager
-  loadFromPreferences(completionHandler:) 

Instance Method

# loadFromPreferences(completionHandler:)

Loads the manager’s saved configuration from the persistent store.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func loadFromPreferences(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func loadFromPreferences() async throws
```

## Parameters 

`completionHandler`  

A completion block that the framework calls after it loads the configuration. If loading failed, the `error` parameter indicates the reason for the failure; otherwise, this parameter is `nil`.

## See Also

### Persisting manager settings

class func loadAllFromPreferences(completionHandler: ([NEAppPushManager]?, (any Error)?) -> Void)

Loads all saved manager configurations asynchronously.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Saves the manager’s configuration in the persistent store.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Removes the manager’s configuration from the persistent store.

