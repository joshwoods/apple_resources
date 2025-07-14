

- SwiftUI
- BackgroundTask
-  urlSession(matching:) 

Type Method

# urlSession(matching:)

A task that responds to background URL sessions matching the given predicate.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func urlSession(matching: @escaping (String) -> Bool) -> BackgroundTask
```

## Parameters 

`matching`  

The predicate to match.

## Return Value

A background task that you can handle with your app or extension.

## See Also

### Responding to URL sessions

static var urlSession: BackgroundTask&lt;String, Void>

A task that responds to background URL sessions.

static func urlSession(String) -> BackgroundTask&lt;Void, Void>

A task that responds to background URL sessions matching the given identifier.

