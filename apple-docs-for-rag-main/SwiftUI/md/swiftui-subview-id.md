

- SwiftUI
- Subview
-  id 

Instance Property

# id

The unique identifier of the view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var id: Subview.ID { get }
```

## Discussion

This identifier persists across updates, changes to the order of subviews, etc. so can be used to track the lifetime of a subview.

