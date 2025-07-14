

- SwiftUI
- VerticalAlignment
-  init(\_:) 

Initializer

# init(\_:)

Creates a custom vertical alignment of the specified type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ id: any AlignmentID.Type)
```

## Parameters 

`id`  

The type of an identifier that uniquely identifies a vertical alignment.

## Discussion

Use this initializer to create a custom vertical alignment. Define an AlignmentID type, and then use that type to create a new static property on VerticalAlignment:

```
private struct FirstThirdAlignment: AlignmentID {
    static func defaultValue(in context: ViewDimensions) -> CGFloat {
        context.height / 3
    }
}

extension VerticalAlignment {
    static let firstThird = VerticalAlignment(FirstThirdAlignment.self)
}
```

Every vertical alignment instance that you create needs a unique identifier. For more information, see AlignmentID.

## See Also

### Creating a custom alignment

func combineExplicit&lt;S>(S) -> CGFloat?

Merges a sequence of explicit alignment values produced by this instance.

