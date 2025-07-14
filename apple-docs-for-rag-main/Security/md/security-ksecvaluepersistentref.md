

- Security
-  kSecValuePersistentRef 

Global Variable

# kSecValuePersistentRef

A key whose value is a persistent reference to the item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecValuePersistentRef: CFString
```

## Discussion

The corresponding value is of type CFData. The bytes in this object can be stored by the caller and used on a subsequent invocation of the application (or even a different application) to retrieve the item referenced by it.

