

- Core Text
-  CTRunDelegateDeallocateCallback 

Type Alias

# CTRunDelegateDeallocateCallback

Defines a pointer to a function that is invoked when a CTRunDelegate object is deallocated.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CTRunDelegateDeallocateCallback = (UnsafeMutableRawPointer) -> Void
```

## Parameters 

`refCon`  

The reference-constant value supplied to the CTRunDelegateCreate(_:_:) function when the run delegate was created.

## Discussion

You would declare the deallocation function like this if you were to name it `MyDeallocationCallback`:

## See Also

### Callbacks

typealias CTRunDelegateGetAscentCallback

Defines a pointer to a function that determines typographic ascent of glyphs in the run.

typealias CTRunDelegateGetDescentCallback

Defines a pointer to a function that determines typographic descent of glyphs in the run.

typealias CTRunDelegateGetWidthCallback

Defines a pointer to a function that determines the typographic width of glyphs in the run.

