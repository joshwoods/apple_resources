

- SwiftUI
- BackgroundTask
-  appRefresh(\_:) 

Type Method

# appRefresh(\_:)

A task that updates your app’s state in the background for a matching identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func appRefresh(_ identifier: String) -> BackgroundTask
```

## Return Value

A background task that you can handle with your app or extension.

## See Also

### Refreshing the app

static var appRefresh: BackgroundTask&lt;String?, Void>

A task that updates your app’s state in the background.

