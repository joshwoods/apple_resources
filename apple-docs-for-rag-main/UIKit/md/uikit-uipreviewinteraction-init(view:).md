

- UIKit
- UIPreviewInteraction
-  init(view:) 

Initializer

# init(view:)

Returns a newly initialized preview interaction for the specified view.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(view: UIView)
```

## Parameters 

`view`  

The view for which the preview interaction should respond.

## Return Value

An initialized preview interaction.

## Discussion

Preview interactions operate on touches within a specified view. Unlike gesture recognizers, the view doesn’t maintain a strong reference to preview interactions. You must therefore retain a reference to the preview interaction to ensure that it continues to receive touches from the view.

