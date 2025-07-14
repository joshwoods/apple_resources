

- Security
-  SecCertificateCopyKey(\_:) 

Function

# SecCertificateCopyKey(\_:)

Retrieves the public key for a given certificate.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func SecCertificateCopyKey(_ certificate: SecCertificate) -> SecKey?
```

## Parameters 

`certificate`  

The certificate from which to copy the key.

## Return Value

The public key. In Objective-C, free this key with a call to the CFRelease function when you are done with it.

## Discussion

The return reference is `NULL` if the public key has an encoding issue or uses an unsupported algorithm.

