

- Core Text
-  CTRunDelegateGetDescentCallback 

Type Alias

# CTRunDelegateGetDescentCallback

Defines a pointer to a function that determines typographic descent of glyphs in the run.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CTRunDelegateGetDescentCallback = (UnsafeMutableRawPointer) -> CGFloat
```

## Parameters 

`refCon`  

The reference-constant value supplied to the CTRunDelegateCreate(_:_:) function when the run delegate was created.

## Return Value

The typographic descent of glyphs in the run associated with the run delegate.

## Discussion

You would declare the get-descent function like this if you were to name it `MyGetDescentCallback`:

## See Also

### Callbacks

typealias CTRunDelegateGetAscentCallback

Defines a pointer to a function that determines typographic ascent of glyphs in the run.

typealias CTRunDelegateGetWidthCallback

Defines a pointer to a function that determines the typographic width of glyphs in the run.

typealias CTRunDelegateDeallocateCallback

Defines a pointer to a function that is invoked when a CTRunDelegate object is deallocated.

