

- Security
-  SecCertificateCopyLongDescription(\_:\_:\_:) 

Function

# SecCertificateCopyLongDescription(\_:\_:\_:)

Returns a copy of the long description of a certificate.

macOS 10.7+

``` source
func SecCertificateCopyLongDescription(
    _ alloc: CFAllocator?,
    _ certificate: SecCertificate,
    _ error: UnsafeMutablePointer?>?
) -> CFString?
```

## Parameters 

`alloc`  

The allocator that should be used. Pass `NULL` or kCFAllocatorDefault to use the default allocator.

`certificate`  

The certificate from which the long description should be copied.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 variable where an error object is stored upon failure. If not `NULL`, the caller is responsible for checking this variable and releasing the resulting object if it exists.

## Return Value

A string object containing the long description, or `NULL` if an error occurred. In Objective-C, free this object with a call to the CFRelease function when you are done with it.

## Discussion

The format of this string is not guaranteed to be consistent across different operating systems or versions. Do not attempt to parse it programmatically.

