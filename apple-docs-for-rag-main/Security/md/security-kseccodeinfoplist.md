

- Security
-  kSecCodeInfoPList 

Global Variable

# kSecCodeInfoPList

A key whose value is an information dictionary containing the contents of the secured `Info.plist` file as seen by Code Signing Services.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCodeInfoPList: CFString
```

## Discussion

The value is a CFDictionary object. Absent if no information property list (`Info.plist`) file is known to Code Signing Services. Note that this is not necessarily the same dictionary as the one that would be returned by a CFBundle function such as CFBundleCopyInfoDictionaryForURL(_:), because CFBundle is free to add entries to the information property list).

This is generic information returned regardless of which Code Signing Information Flags you pass to the SecCodeCopySigningInformation(_:_:_:) function.

