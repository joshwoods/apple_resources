

- SwiftUI
- BackgroundTask
-  appRefresh 

Type Property

# appRefresh

A task that updates your app’s state in the background.

watchOS 9.0+

``` source
static var appRefresh: BackgroundTask { get }
```

## See Also

### Refreshing the app

static func appRefresh(String) -> BackgroundTask&lt;Void, Void>

A task that updates your app’s state in the background for a matching identifier.

