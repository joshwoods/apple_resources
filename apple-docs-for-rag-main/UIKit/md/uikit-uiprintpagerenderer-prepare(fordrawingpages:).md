

- UIKit
- UIPrintPageRenderer
-  prepare(forDrawingPages:) 

Instance Method

# prepare(forDrawingPages:)

Prepares the renderer for drawing a range of pages.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func prepare(forDrawingPages range: NSRange)
```

## Parameters 

`range`  

A range of pages.

## Discussion

UIKit calls this method before it requests drawing for a range of pages. You can optionally override this method to perform setup tasks. The default implementation does nothing.

