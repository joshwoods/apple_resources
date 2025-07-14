

- Security
-  CMSEncoderCreate(\_:) 

Function

# CMSEncoderCreate(\_:)

Creates a CMSEncoder reference.

macOS 10.5+

``` source
func CMSEncoderCreate(_ cmsEncoderOut: UnsafeMutablePointer) -> OSStatus
```

## Parameters 

`cmsEncoderOut`  

On return, points to a CMSEncoder reference. You must use the `CFRelease` function to free this reference when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

This is the first function in a sequence of encoder functions that you call to sign or encrypt a message. The other functions in the sequence require you to pass in the CMSEncoder reference returned by this function. In many cases, you can call the CMSEncode function alone instead of this sequence of encoder functions.

