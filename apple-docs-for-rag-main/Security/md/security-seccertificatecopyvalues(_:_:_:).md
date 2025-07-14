

- Security
-  SecCertificateCopyValues(\_:\_:\_:) 

Function

# SecCertificateCopyValues(\_:\_:\_:)

Creates a dictionary that represents a certificate’s contents.

macOS 10.7+

``` source
func SecCertificateCopyValues(
    _ certificate: SecCertificate,
    _ keys: CFArray?,
    _ error: UnsafeMutablePointer?>?
) -> CFDictionary?
```

## Parameters 

`certificate`  

The certificate from which values should be copied.

`keys`  

An array of string OID values, or `NULL`. If non-`NULL`, these OID values determine which values from the certificate to return. If `NULL`, all values are returned.

Only OIDs that represent top-level keys in the returned dictionary can be specified. Unknown OIDs are ignored. See Certificate OIDs for the list of known OIDs.

`error`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 variable where an error object is stored upon failure. If not `NULL`, the caller is responsible for checking this variable and releasing the resulting object if it exists.

## Return Value

A dictionary containing the specified values from the certificate or `NULL` if an error occurs. In Objective-C, free this dictionary with a call to the CFRelease function when you are done with it.

## Mentioned in 

Getting Certificate Values

## Discussion

Each entry in this dictionary is itself a dictionary with the keys described in Certificate Property Keys.

