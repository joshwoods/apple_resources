

- AppKit
- NSEPSImageRep
-  prepareGState() Deprecated

Instance Method

# prepareGState()

Implemented by subclasses to configure the graphics state prior to drawing.

macOS 10.0–10.10Deprecated

``` source
func prepareGState()
```

## Discussion

The draw() method of NSEPSImageRep sends this message to itself just before rendering the EPS code. The default implementation of this method does nothing. You can override it in your subclass to prepare the graphics state as needed.

