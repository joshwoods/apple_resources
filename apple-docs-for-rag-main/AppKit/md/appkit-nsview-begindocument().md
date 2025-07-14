

- AppKit
- NSView
-  beginDocument() 

Instance Method

# beginDocument()

Invoked at the beginning of the printing session, this method sets up the current graphics context.

macOS

``` source
@MainActor
func beginDocument()
```

## Discussion

Note that this method may be invoked in a subthread.

Override it to configure printing related settings. You should store your settings in the object returned by `NSPrintInfo`’s shared class method, which is guaranteed to return an instance specific to the thread in which you invoke this method. If you override this method, call the superclass implementation.

## See Also

### Writing Conforming Rendering Instructions

func endDocument()

This method is invoked at the end of the printing session.

func endPage()

Writes the end of a conforming page.

