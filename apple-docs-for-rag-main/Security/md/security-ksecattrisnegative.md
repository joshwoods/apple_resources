

- Security
-  kSecAttrIsNegative 

Global Variable

# kSecAttrIsNegative

A key with a value that’s a Boolean indicating whether the item has a valid password.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrIsNegative: CFString
```

## Discussion

The corresponding value is of type CFBoolean and indicates whether there is a valid password associated with this keychain item. This is useful if your application doesn’t want a password for some particular service to be stored in the keychain, but prefers that it always be entered by the user.

