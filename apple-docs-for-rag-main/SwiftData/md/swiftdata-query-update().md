

- SwiftData
- Query
-  update() 

Instance Method

# update()

Updates the underlying value of the stored value.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func update()
```

## Discussion

SwiftUI calls this function before rendering a view’s `View/body-swift.property` to ensure the view has the most recent value.

