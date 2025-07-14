

- Security
-  SecCopyErrorMessageString(\_:\_:) 

Function

# SecCopyErrorMessageString(\_:\_:)

Returns a string explaining the meaning of a security result code.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+macOS 10.3+tvOS 11.3+visionOS 1.0+watchOS 4.3+

``` source
func SecCopyErrorMessageString(
    _ status: OSStatus,
    _ reserved: UnsafeMutableRawPointer?
) -> CFString?
```

## Parameters 

`status`  

A result code of type `OSStatus` returned by a security function. See Security Framework Result Codes for a list of codes.

`reserved`  

Reserved for future use. Pass `nil` for this parameter.

## Return Value

A human-readable string describing the result, or `nil` if no string is available for the specified result code. In Objective-C, call the CFRelease function to release this object when you are finished using it.

