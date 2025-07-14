

- Core Graphics
- CGContext
-  beginPage(mediaBox:) 

Instance Method

# beginPage(mediaBox:)

Starts a new page in a page-based graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func beginPage(mediaBox: UnsafePointer?)
```

## Parameters 

`mediaBox`  

A rectangle defining the bounds of the new page, expressed in units of the default user space, or `NULL`. These bounds supersede any supplied for the media box when you created the context. If you pass `NULL`, Core Graphics uses the rectangle you supplied for the media box when the graphics context was created.

## Discussion

When using a graphics context that supports multiple pages, you should call this function together with endPage() to delineate the page boundaries in the output. In other words, each page should be bracketed by calls to `CGContextBeginPage` and `CGContextEndPage`. Core Graphics ignores all drawing operations performed outside a page boundary in a page-based context.

## See Also

### Managing a Page-Based Graphics Context

func endPage()

Ends the current page in a page-based graphics context.

