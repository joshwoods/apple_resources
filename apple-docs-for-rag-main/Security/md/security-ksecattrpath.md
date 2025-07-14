

- Security
-  kSecAttrPath 

Global Variable

# kSecAttrPath

A key whose value is a string indicating the item’s path attribute.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrPath: CFString
```

## Discussion

The corresponding value is of type CFString and represents a path, typically the path component of the URL. Items of class kSecClassInternetPassword have this attribute.

