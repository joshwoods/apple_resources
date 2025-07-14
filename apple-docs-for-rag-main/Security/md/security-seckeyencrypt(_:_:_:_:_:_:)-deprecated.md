

- Security
-  SecKeyEncrypt(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# SecKeyEncrypt(\_:\_:\_:\_:\_:\_:)

Encrypts a block of plaintext.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 4.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–8.0Deprecated

``` source
func SecKeyEncrypt(
    _ key: SecKey,
    _ padding: SecPadding,
    _ plainText: UnsafePointer,
    _ plainTextLen: Int,
    _ cipherText: UnsafeMutablePointer,
    _ cipherTextLen: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

Use SecKeyCreateEncryptedData

## Parameters 

`key`  

Public key with which to encrypt the data.

`padding`  

The type of padding to use. Possible values are listed in SecPadding. Typically, PKCS1 is used, which adds PKCS1 padding before encryption. If you specify kSecPaddingNone, the data is encrypted as-is.

`plainText`  

The data to encrypt.

`plainTextLen`  

Length in bytes of the data in the `plainText` buffer. This must be less than or equal to the value returned by the SecKeyGetBlockSize(_:) function. When PKCS1 padding is performed, the maximum length of data that can be encrypted is 11 bytes less than the value returned by the SecKeyGetBlockSize(_:) function (`secKeyGetBlockSize() - 11`).

`cipherText`  

On return, the encrypted text.

`cipherTextLen`  

On entry, the size of the buffer provided in the `cipherText` parameter. On return, the amount of data actually placed in the buffer.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

The input buffer (`plainText`) can be the same as the output buffer (`cipherText`) to reduce the amount of memory used by the function.

