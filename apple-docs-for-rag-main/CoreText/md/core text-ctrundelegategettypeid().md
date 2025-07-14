

- Core Text
-  CTRunDelegateGetTypeID() 

Function

# CTRunDelegateGetTypeID()

Returns the type of CTRunDelegate objects.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRunDelegateGetTypeID() -> CFTypeID
```

## Discussion

The return type is a Core Foundation type (CTType).

## See Also

### Getting Information About a Run Delegate

func CTRunDelegateGetRefCon(CTRunDelegate) -> UnsafeMutableRawPointer

Returns a run delegate’s “refCon” value.

