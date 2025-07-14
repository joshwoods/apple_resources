

- Security
-  kSecSharedPassword 

Global Variable

# kSecSharedPassword

A dictionary key whose value is the shared password.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
let kSecSharedPassword: CFString
```

## Discussion

The dictionary returned by the SecRequestSharedWebCredential(_:_:_:) function includes this key to provide you with the password.

You can also access the server’s URL and the user name from this dictionary. To access the server, use the kSecAttrServer constant. To access the user name, use the kSecAttrAccount constant. These constants are part of the Keychain services API, and in particular are listed among the Item attribute keys and values.

