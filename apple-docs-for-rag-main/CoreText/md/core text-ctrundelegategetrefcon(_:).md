

- Core Text
-  CTRunDelegateGetRefCon(\_:) 

Function

# CTRunDelegateGetRefCon(\_:)

Returns a run delegate’s “refCon” value.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTRunDelegateGetRefCon(_ runDelegate: CTRunDelegate) -> UnsafeMutableRawPointer
```

## Parameters 

`runDelegate`  

The run delegate object being queried.

## Return Value

A constant value associated with the run delegate as an identifier.

## Discussion

The run delegate object was created with the returned “refCon” value.

## See Also

### Getting Information About a Run Delegate

func CTRunDelegateGetTypeID() -> CFTypeID

Returns the type of CTRunDelegate objects.

