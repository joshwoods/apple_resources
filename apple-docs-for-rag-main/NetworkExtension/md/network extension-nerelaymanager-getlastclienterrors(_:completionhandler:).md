

- Network Extension
- NERelayManager
-  getLastClientErrors(\_:completionHandler:) 

Instance Method

# getLastClientErrors(\_:completionHandler:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func getLastClientErrors(
    _ seconds: TimeInterval,
    completionHandler: @escaping ([any Error]?) -> Void
)
```

``` source
func lastClientErrors(_ seconds: TimeInterval) async -> [any Error]?
```

