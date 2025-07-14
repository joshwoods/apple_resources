

- Assignables
- AssignableDocumentView
-  contentShape(\_:eoFill:) 

Instance Method

# contentShape(\_:eoFill:)

Defines the content shape for hit testing.

AssignablesSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func contentShape(
    _ shape: S,
    eoFill: Bool = false
) -> some View where S : Shape
```

## Parameters 

`shape`  

The hit testing shape for the view.

`eoFill`  

A Boolean that indicates whether the shape is interpreted with the even-odd winding number rule.

## Return Value

A view that uses the given shape for hit testing.

