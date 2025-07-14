

- Core Graphics
- CGContext
-  endPage() 

Instance Method

# endPage()

Ends the current page in a page-based graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func endPage()
```

## Discussion

When using a graphics context that supports multiple pages, you should call this function to terminate drawing in the current page.

## See Also

### Managing a Page-Based Graphics Context

func beginPage(mediaBox: UnsafePointer&lt;CGRect>?)

Starts a new page in a page-based graphics context.

