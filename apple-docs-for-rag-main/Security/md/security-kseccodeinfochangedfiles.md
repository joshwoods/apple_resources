

- Security
-  kSecCodeInfoChangedFiles 

Global Variable

# kSecCodeInfoChangedFiles

A key whose value is a list of all files in the code that may have been modified by the process of signing it.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoChangedFiles: CFString
```

## Discussion

The value is a CFArray array of CFURL objects. Files not in this list have not been touched by the signing operation.

Specify the kSecCSContentInformation flag when calling the SecCodeCopySigningInformation(_:_:_:) function to get this information.

