

- Network Extension
- NERelayManager
-  loadAllManagersFromPreferences(completionHandler:) 

Type Method

# loadAllManagersFromPreferences(completionHandler:)

Asynchronously reads all the relay configurations previously created and saved by the calling app.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class func loadAllManagersFromPreferences(completionHandler: @escaping ([NERelayManager], (any Error)?) -> Void)
```

``` source
class func loadAllManagersFromPreferences() async throws -> [NERelayManager]
```

## Parameters 

`completionHandler`  

A block that receives an array of NERelayManager objects. If the system failed to read any NERelay configurations read from the disk, the array is passes to the block is empty. The NSError passed to this block is `nil` if the load operation succeeded, non-`nil` otherwise.

