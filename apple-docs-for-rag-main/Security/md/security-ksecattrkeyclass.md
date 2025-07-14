

- Security
-  kSecAttrKeyClass 

Global Variable

# kSecAttrKeyClass

A key whose value indicates the item’s cryptographic key class.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrKeyClass: CFString
```

## Discussion

The corresponding value is of type CFTypeRef and specifies a type of cryptographic key. Possible values are listed in Key Class Values. Read only.

Note

Don’t confuse this attribute with the more general kSecClass attribute that indicates an item’s class (for example password, certificate, or cryptographic key). The kSecAttrKeyClass attribute described here applies only to items of class kSecClassKey, indicating what category a cryptographic key fits into (for example, public, private, or symmetric).

