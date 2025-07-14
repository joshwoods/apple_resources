

- Security
-  SecTrustedApplicationCreateFromPath(\_:\_:) Deprecated

Function

# SecTrustedApplicationCreateFromPath(\_:\_:)

Creates a trusted app instance based on the app at the given path in the file system.

macOS 10.0–10.10Deprecated

``` source
func SecTrustedApplicationCreateFromPath(
    _ path: UnsafePointer?,
    _ app: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`path`  

The path to the app to trust. For application bundles, use the path to the bundle directory. Pass `nil` to refer to the calling app.

`app`  

On return, points to the newly created trusted app instance. Call the CFRelease method to release this instance when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

Use this method to create a trusted app instance, which both identifies an app and provides data that can be used to ensure that the app hasn’t been altered since the instance was created.

You can use the created instance as input to the SecAccessCreate(_:_:_:) method, which creates an access instance. The access instance, in turn, is used as input to the SecKeychainItemSetAccess(_:_:) function to specify the set of apps that are trusted to access a specific keychain item.

