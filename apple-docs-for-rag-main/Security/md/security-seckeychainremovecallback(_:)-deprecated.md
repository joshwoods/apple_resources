

- Security
-  SecKeychainRemoveCallback(\_:) Deprecated

Function

# SecKeychainRemoveCallback(\_:)

Unregisters your keychain event callback function.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainRemoveCallback(_ callbackFunction: SecKeychainCallback) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`callbackFunction`  

The callback function pointer to remove.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Once removed, keychain events are not sent to the owner of the callback.

