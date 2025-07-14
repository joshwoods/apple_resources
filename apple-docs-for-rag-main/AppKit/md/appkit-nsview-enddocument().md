

- AppKit
- NSView
-  endDocument() 

Instance Method

# endDocument()

This method is invoked at the end of the printing session.

macOS

``` source
@MainActor
func endDocument()
```

## Discussion

If you override this method, call the superclass implementation.

## See Also

### Writing Conforming Rendering Instructions

func beginDocument()

Invoked at the beginning of the printing session, this method sets up the current graphics context.

func endPage()

Writes the end of a conforming page.

