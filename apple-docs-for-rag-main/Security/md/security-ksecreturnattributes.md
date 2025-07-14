

- Security
-  kSecReturnAttributes 

Global Variable

# kSecReturnAttributes

A key whose value is a Boolean indicating whether or not to return item attributes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecReturnAttributes: CFString
```

## Discussion

The corresponding value is of type CFBoolean. A value of kCFBooleanTrue indicates that a dictionary of the (unencrypted) attributes of an item should be returned in the form of a CFDictionary using the keys and values defined in Item attribute keys and values.

