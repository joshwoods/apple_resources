

- Security
-  kSecCFErrorGuestAttributes 

Global Variable

# kSecCFErrorGuestAttributes

A key whose value is a Core Foundation object containing an attribute that is unrecognized or that contains a value of the wrong type.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCFErrorGuestAttributes: CFString
```

## Discussion

This key is present when you pass a bad guest attribute to the SecHostCreateGuest or SecHostSetGuestStatus function.

