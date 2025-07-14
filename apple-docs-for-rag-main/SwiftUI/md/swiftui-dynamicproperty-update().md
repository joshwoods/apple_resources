

- SwiftUI
- DynamicProperty
-  update() 

Instance Method

# update()

Updates the underlying value of the stored value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func update()
```

**Required** Default implementation provided.

## Discussion

SwiftUI calls this function before rendering a view’s body to ensure the view has the most recent value.

## Default Implementations

### DynamicProperty Implementations

func update()

Updates the underlying value of the stored value.

