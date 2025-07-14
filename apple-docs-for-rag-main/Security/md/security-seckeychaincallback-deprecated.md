

- Security
-  SecKeychainCallback Deprecated

Type Alias

# SecKeychainCallback

A customized callback function that keychain services call when a keychain event has occurred.

macOS 10.2–10.10Deprecated

``` source
typealias SecKeychainCallback = (SecKeychainEvent, UnsafeMutablePointer, UnsafeMutableRawPointer?) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`keychainEvent`  

The keychain event that occurred. The type of event that can trigger your callback depends on the bit mask you passed in the `eventMask` parameter of the function SecKeychainAddCallback(_:_:_:). See SecKeychainEvent for a list of possible values.

`info`  

A pointer to a structure of type SecKeychainCallbackInfo. This structure provides your callback with information about the keychain event.

`context`  

A pointer to application-defined storage that your application previously passed to the function SecKeychainAddCallback(_:_:_:). You can use this value to provide information that the callback function needs in order to properly handle the event, such as an object on which the callback function should call a method.

## Return Value

A result code. See `Codes`.

## Discussion

You would declare your keychain callback function like this if you were to name it `MyKeychainCallback`:

Listing 1. Declaring a keychain callback function

```
OSStatus MyKeychainCallback (
    SecKeychainEvent keychainEvent,
    SecKeychainCallbackInfo *info,
    void *context
);
```

To add your callback function, use the SecKeychainAddCallback(_:_:_:) function. To remove your callback function, use the SecKeychainRemoveCallback(_:) function.

