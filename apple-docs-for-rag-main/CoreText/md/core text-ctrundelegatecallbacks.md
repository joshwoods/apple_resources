

- Core Text
-  CTRunDelegateCallbacks 

Structure

# CTRunDelegateCallbacks

A structure holding pointers to callbacks implemented by the run delegate.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CTRunDelegateCallbacks
```

## Overview

You pass in a pointer to this structure when you create a CTRunDelegate object with the CTRunDelegateCreate(_:_:) function. The callbacks defined in this structure are provided by the owner of a run delegate and are used to modify glyph metrics during layout. The values returned by the delegate are applied to each glyph in the run or runs corresponding to the attribute containing that delegate.

See CTRunDelegate for a discussion of the function-pointer types associated with these callbacks.

## Topics

### Initializers

init(version: CFIndex, dealloc: CTRunDelegateDeallocateCallback, getAscent: CTRunDelegateGetAscentCallback, getDescent: CTRunDelegateGetDescentCallback, getWidth: CTRunDelegateGetWidthCallback)

### Instance Properties

var dealloc: CTRunDelegateDeallocateCallback

The callback invoked when the retain count of a CTRunDelegate reaches 0 and the CTRunDelegate is deallocated. This callback may be `NULL`.

var getAscent: CTRunDelegateGetAscentCallback

The callback invoked to request the run delegate to determine and return the typographic ascent of glyphs in the run. This callback may be `NULL`, which is equivalent to a `getAscent` callback that always returns 0.

var getDescent: CTRunDelegateGetDescentCallback

The callback invoked to request the run delegate to determine and return the typographic descent of glyphs in the run. This callback may be `NULL`, which is equivalent to a `getDescent` callback that always returns 0.

var getWidth: CTRunDelegateGetWidthCallback

The callback invoked to request the run delegate to determine and return the typographic width of glyphs in the run. This callback may be `NULL`, which is equivalent to a `getWidth` callback that always returns 0.

var version: CFIndex

The version number of the callbacks being passed in as a parameter to CTRunDelegateCreate(_:_:). The initial version is kCTRunDelegateVersion1.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

