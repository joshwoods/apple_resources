

- AppKit
- NSView
-  endPage() 

Instance Method

# endPage()

Writes the end of a conforming page.

macOS

``` source
@MainActor
func endPage()
```

## Discussion

This method is invoked after each page is printed. It invokes unlockFocus(). This method also generates comments for the bounding box and page fonts, if they were specified as being at the end of the page.

## See Also

### Writing Conforming Rendering Instructions

func beginDocument()

Invoked at the beginning of the printing session, this method sets up the current graphics context.

func endDocument()

This method is invoked at the end of the printing session.

