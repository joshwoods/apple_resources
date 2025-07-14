

- Core Text
-  CTRunDelegateGetWidthCallback 

Type Alias

# CTRunDelegateGetWidthCallback

Defines a pointer to a function that determines the typographic width of glyphs in the run.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CTRunDelegateGetWidthCallback = (UnsafeMutableRawPointer) -> CGFloat
```

## Parameters 

`refCon`  

The reference-constant value supplied to the CTRunDelegateCreate(_:_:) function when the run delegate was created.

## Return Value

The typographic width of glyphs in the run associated with the run delegate. A value of 0.0 indicates that the glyphs should not be drawn.

## Discussion

You would declare the get-width function like this if you were to name it `MyGetWidthCallback`:

## See Also

### Callbacks

typealias CTRunDelegateGetAscentCallback

Defines a pointer to a function that determines typographic ascent of glyphs in the run.

typealias CTRunDelegateGetDescentCallback

Defines a pointer to a function that determines typographic descent of glyphs in the run.

typealias CTRunDelegateDeallocateCallback

Defines a pointer to a function that is invoked when a CTRunDelegate object is deallocated.

