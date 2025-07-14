

- Security
-  SecKeychainCallbackInfo 

Structure

# SecKeychainCallbackInfo

Information about a keychain event that keychain services deliver to your app via a callback function.

macOS 10.0+

``` source
struct SecKeychainCallbackInfo
```

## Overview

This structure contains information about the keychain event of which your application wants to be notified. Keychain services pass a pointer to this structure in the `info` parameter of your callback function. For information on how to write a keychain event callback function, see SecKeychainCallback.

## Topics

### Instance Properties

var item: Unmanaged&lt;SecKeychainItem>

A reference to the keychain item in which the event occurred. If the event did not involve an item, this field is not valid.

var keychain: Unmanaged&lt;SecKeychain>

A reference to the keychain in which the event occurred. If the event did not involve a keychain, this field is not valid.

var pid: pid_t

The ID of the process that generated this event.

var version: UInt32

The version of this structure.

### Initializers

init(version: UInt32, item: Unmanaged&lt;SecKeychainItem>, keychain: Unmanaged&lt;SecKeychain>, pid: pid_t)

Creates a new keychain callback information structure.

## Relationships

### Conforms To

- BitwiseCopyable

