

- AppKit
- NSGraphicsContext
-  flushGraphics() 

Instance Method

# flushGraphics()

Forces any buffered operations or data to be sent to the graphics context’s destination.

macOS

``` source
func flushGraphics()
```

## Discussion

Graphics contexts use buffers to queue pending operations but for efficiency reasons may not always empty those buffers immediately. This method forces the buffers to be emptied.

