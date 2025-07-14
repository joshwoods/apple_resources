

- Core Text
-  CTRunDelegateGetAscentCallback 

Type Alias

# CTRunDelegateGetAscentCallback

Defines a pointer to a function that determines typographic ascent of glyphs in the run.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CTRunDelegateGetAscentCallback = (UnsafeMutableRawPointer) -> CGFloat
```

## Parameters 

`refCon`  

The reference-constant value supplied to the CTRunDelegateCreate(_:_:) function when the run delegate was created.

## Return Value

The typographic ascent of glyphs in the run associated with the run delegate.

## Discussion

You would declare the get-ascent function like this if you were to name it `MyGetAscentCallback`:

## See Also

### Callbacks

typealias CTRunDelegateGetDescentCallback

Defines a pointer to a function that determines typographic descent of glyphs in the run.

typealias CTRunDelegateGetWidthCallback

Defines a pointer to a function that determines the typographic width of glyphs in the run.

typealias CTRunDelegateDeallocateCallback

Defines a pointer to a function that is invoked when a CTRunDelegate object is deallocated.

