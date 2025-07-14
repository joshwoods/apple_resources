

- Security
-  CMSDecoderSetSearchKeychain(\_:\_:) Deprecated

Function

# CMSDecoderSetSearchKeychain(\_:\_:)

Specifies the keychains to search for intermediate certificates to be used in verifying a signed message’s signer certificates.

macOS 10.5–10.13Deprecated

``` source
func CMSDecoderSetSearchKeychain(
    _ cmsDecoder: CMSDecoder,
    _ keychainOrArray: CFTypeRef
) -> OSStatus
```

## Parameters 

`cmsDecoder`  

The CMSDecoder reference returned by the `CMSDecoderCreate` function.

`keychainOrArray`  

Either a single keychain to search, specified as a keychain object (type `SecKeychainRef`), or a set of keychains specified as a `CFArray` of keychain objects. If you specify an empty `CFArrayRef`, no keychains are searched for intermediate certificates.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

If you don’t call this function, the decoder uses the default keychain search list to search for intermediate certificates.

If you do call this function, you must call it before you call the `CMSDecoderCopySignerStatus` function.

## See Also

### Related Documentation

func CMSDecoderCreate(UnsafeMutablePointer&lt;CMSDecoder?>) -> OSStatus

Creates a CMSDecoder reference.

