

- Network Extension
- NETransparentProxyManager
-  loadAllFromPreferences(completionHandler:) 

Type Method

# loadAllFromPreferences(completionHandler:)

Loads all previously-saved transparent proxy configurations.

macOS 10.15+

``` source
class func loadAllFromPreferences(completionHandler: @escaping ([NETransparentProxyManager]?, (any Error)?) -> Void)
```

``` source
class func loadAllFromPreferences() async throws -> [NETransparentProxyManager]
```

## Parameters 

`completionHandler`  

A Swift closure or an ObjectiveC block that receives as parameters an array of transparent proxy manager instances loaded from disk and an error. If the error is `nil`, no error occurred.

## Discussion

This method asychronously reads all previously-saved transparent proxy configurations associated with the calling app.

