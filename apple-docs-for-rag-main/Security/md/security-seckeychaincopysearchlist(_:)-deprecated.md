

- Security
-  SecKeychainCopySearchList(\_:) Deprecated

Function

# SecKeychainCopySearchList(\_:)

Retrieves a keychain search list.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainCopySearchList(_ searchList: UnsafeMutablePointer) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`searchList`  

On return, the returned keychain search list. In Objective-C, call the CFRelease function to release this object when you are finished using it.

## Return Value

A result code. See Security Framework Result Codes.

