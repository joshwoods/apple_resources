

- Security
-  kSecCodeInfoMainExecutable 

Global Variable

# kSecCodeInfoMainExecutable

A key whose value is a URL locating the main executable file of the code.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoMainExecutable: CFString
```

## Discussion

The value is a CFURL object. For single files, the URL locates the file itself. For bundles, it locates the main executable as identified by the bundle’s `Info.plist` file.

This is generic information returned regardless of which Code Signing Information Flags you pass to the SecCodeCopySigningInformation(_:_:_:) function.

