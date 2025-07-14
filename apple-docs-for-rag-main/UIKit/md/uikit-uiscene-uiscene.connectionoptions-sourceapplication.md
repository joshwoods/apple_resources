

- UIKit
- UIScene
- UIScene.ConnectionOptions
-  sourceApplication 

Instance Property

# sourceApplication

The bundle ID of the app that originated the request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var sourceApplication: String? { get }
```

## Discussion

If the request originated from another app belonging to your team, UIKit places the bundle ID of that app in this property. If the team identifier of the originating app is different than the team identifier of the current app, this property is `nil`.

