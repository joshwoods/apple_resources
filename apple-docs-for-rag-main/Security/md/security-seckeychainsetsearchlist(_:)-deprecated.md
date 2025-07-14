

- Security
-  SecKeychainSetSearchList(\_:) Deprecated

Function

# SecKeychainSetSearchList(\_:)

Specifies the list of keychains to use in the default keychain search list.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainSetSearchList(_ searchList: CFArray) -> OSStatus
```

Deprecated

SecKeychain is deprecated

## Parameters 

`searchList`  

An array of keychain references (of type SecKeychain) specifying the list of keychains to use in the default keychain search list. Passing an empty array clears the search list.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

The default keychain search list is used by several functions; see for example SecKeychainSearchCreateFromAttributes, SecKeychainFindInternetPassword(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:), or SecKeychainFindGenericPassword(_:_:_:_:_:_:_:_:). To obtain the current default keychain search list, use the SecKeychainCopySearchList(_:) function.

The default keychain search list is displayed as the keychain list in the Keychain Access utility. If you use SecKeychainSetSearchList(_:) to change the keychain search list, the list displayed in Keychain Access changes accordingly.

