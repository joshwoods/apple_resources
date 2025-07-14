

- Network Extension
- NEAppPushManager
-  loadAllFromPreferences(completionHandler:) 

Type Method

# loadAllFromPreferences(completionHandler:)

Loads all saved manager configurations asynchronously.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
class func loadAllFromPreferences(completionHandler: @escaping ([NEAppPushManager]?, (any Error)?) -> Void)
```

``` source
class func loadAllFromPreferences() async throws -> [NEAppPushManager]
```

## Parameters 

`completionHandler`  

A completion block that the framework calls after it loads the configurations. The `managers` parameter contains an array of all managers that the framework loads from the persistent store. This array is empty if the framework didn’t load any configurations. If loading failed, the `error` parameter indicates the reason for the failure; otherwise, this parameter is `nil`.

## See Also

### Persisting manager settings

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Loads the manager’s saved configuration from the persistent store.

func saveToPreferences(completionHandler: ((any Error)?) -> Void)

Saves the manager’s configuration in the persistent store.

func removeFromPreferences(completionHandler: ((any Error)?) -> Void)

Removes the manager’s configuration from the persistent store.

