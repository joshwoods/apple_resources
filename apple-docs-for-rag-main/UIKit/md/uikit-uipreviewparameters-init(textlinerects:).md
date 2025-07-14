

- UIKit
- UIPreviewParameters
-  init(textLineRects:) 

Initializer

# init(textLineRects:)

Creates a preview parameters object with information about the text you want to preview.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
convenience init(textLineRects: [NSValue])
```

## Parameters 

`textLineRects`  

An array of text line rectangles in the coordinate system of the view being animated. UIKit clips the previewed content using the specified rectangles. Wrap each CGRect in an NSValue object. If you specify an empty array, UIKit shows the entire view.

## Return Value

A new preview parameters object for a view containing text.

## See Also

### Creating preview parameters

init()

Creates a default set of preview parameters.

