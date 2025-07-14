

- SwiftUI
- HorizontalAlignment
-  init(\_:) 

Initializer

# init(\_:)

Creates a custom horizontal alignment of the specified type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ id: any AlignmentID.Type)
```

## Parameters 

`id`  

The type of an identifier that uniquely identifies a horizontal alignment.

## Discussion

Use this initializer to create a custom horizontal alignment. Define an AlignmentID type, and then use that type to create a new static property on HorizontalAlignment:

```
private struct OneQuarterAlignment: AlignmentID {
    static func defaultValue(in context: ViewDimensions) -> CGFloat {
        context.width / 4
    }
}

extension HorizontalAlignment {
    static let oneQuarter = HorizontalAlignment(OneQuarterAlignment.self)
}
```

Every horizontal alignment instance that you create needs a unique identifier. For more information, see AlignmentID.

## See Also

### Creating a custom alignment

func combineExplicit&lt;S>(S) -> CGFloat?

Merges a sequence of explicit alignment values produced by this instance.

