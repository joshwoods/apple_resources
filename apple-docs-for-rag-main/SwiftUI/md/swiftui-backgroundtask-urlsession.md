

- SwiftUI
- BackgroundTask
-  urlSession 

Type Property

# urlSession

A task that responds to background URL sessions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var urlSession: BackgroundTask { get }
```

## See Also

### Responding to URL sessions

static func urlSession(String) -> BackgroundTask&lt;Void, Void>

A task that responds to background URL sessions matching the given identifier.

static func urlSession(matching: (String) -> Bool) -> BackgroundTask&lt;String, Void>

A task that responds to background URL sessions matching the given predicate.

