

- Security
-  SecKeyDecrypt(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# SecKeyDecrypt(\_:\_:\_:\_:\_:\_:)

Decrypts a block of ciphertext.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 4.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–8.0Deprecated

``` source
func SecKeyDecrypt(
    _ key: SecKey,
    _ padding: SecPadding,
    _ cipherText: UnsafePointer,
    _ cipherTextLen: Int,
    _ plainText: UnsafeMutablePointer,
    _ plainTextLen: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

Use SecKeyCreateDecryptedData

## Parameters 

`key`  

Private key with which to decrypt the data.

`padding`  

The type of padding used. Possible values are listed in SecPadding. Typically, PKCS1 is used, which removes PKCS1 padding after decryption. If you specify kSecPaddingNone, the decrypted data is returned as-is.

`cipherText`  

The data to decrypt.

`cipherTextLen`  

Length in bytes of the data in the `cipherText` buffer. This must be less than or equal to the value returned by the SecKeyGetBlockSize(_:) function.

`plainText`  

On return, the decrypted text.

`plainTextLen`  

On entry, the size of the buffer provided in the `plainText` parameter. On return, the amount of data actually placed in the buffer.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

The input buffer (`cipherText`) can be the same as the output buffer (`plainText`) to reduce the amount of memory used by the function.

