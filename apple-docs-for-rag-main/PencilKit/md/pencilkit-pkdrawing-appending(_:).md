

- PencilKit
- PKDrawing
-  appending(\_:) 

Instance Method

# appending(\_:)

Returns a new drawing created by appending the current drawing with another drawing you provide.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
func appending(_ toAppend: PKDrawing) -> PKDrawing
```

## Parameters 

`toAppend`  

A drawing object that contains additional content.

## Return Value

A new drawing created by merging the content from the current object with the content in the drawing parameter.

## See Also

### Modifying the drawing

func transform(using: CGAffineTransform)

Applies the specified transform to the contents of this drawing.

func transformed(using: CGAffineTransform) -> PKDrawing

Applies the specified transform and returns a new drawing.

func append(PKDrawing)

Appends the contents of the specified drawing object to an existing drawing object that you provide.

