

- UIKit
- UIDropSession
-  localDragSession 

Instance Property

# localDragSession

The drag session that corresponds to this drop session, for in-app drag activities.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var localDragSession: (any UIDragSession)? { get }
```

**Required**

## Discussion

The local drag session is `nil` if the drag activity started in a different app.

