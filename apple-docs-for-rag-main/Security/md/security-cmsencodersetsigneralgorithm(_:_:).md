

- Security
-  CMSEncoderSetSignerAlgorithm(\_:\_:) 

Function

# CMSEncoderSetSignerAlgorithm(\_:\_:)

Sets the digest algorithm to use for the signer.

macOS 10.11+

``` source
func CMSEncoderSetSignerAlgorithm(
    _ cmsEncoder: CMSEncoder,
    _ digestAlgorithm: CFString
) -> OSStatus
```

## Parameters 

`cmsEncoder`  

The CMSEncoder reference returned by the CMSEncoderCreate(_:) function.

`digestAlgorithm`  

A string representing the digest algorithm to use.

## Return Value

A result code. See Security Framework Result Codes.

