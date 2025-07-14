

- Core Text
- CTRunDelegateCallbacks
-  getDescent 

Instance Property

# getDescent

The callback invoked to request the run delegate to determine and return the typographic descent of glyphs in the run. This callback may be `NULL`, which is equivalent to a `getDescent` callback that always returns 0.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var getDescent: CTRunDelegateGetDescentCallback
```

## See Also

### Instance Properties

var dealloc: CTRunDelegateDeallocateCallback

The callback invoked when the retain count of a CTRunDelegate reaches 0 and the CTRunDelegate is deallocated. This callback may be `NULL`.

var getAscent: CTRunDelegateGetAscentCallback

The callback invoked to request the run delegate to determine and return the typographic ascent of glyphs in the run. This callback may be `NULL`, which is equivalent to a `getAscent` callback that always returns 0.

var getWidth: CTRunDelegateGetWidthCallback

The callback invoked to request the run delegate to determine and return the typographic width of glyphs in the run. This callback may be `NULL`, which is equivalent to a `getWidth` callback that always returns 0.

var version: CFIndex

The version number of the callbacks being passed in as a parameter to CTRunDelegateCreate(_:_:). The initial version is kCTRunDelegateVersion1.

