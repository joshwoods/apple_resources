

- Security
-  SecKeyRawSign(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# SecKeyRawSign(\_:\_:\_:\_:\_:\_:)

Generates a digital signature for a block of data.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 4.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–8.0Deprecated

``` source
func SecKeyRawSign(
    _ key: SecKey,
    _ padding: SecPadding,
    _ dataToSign: UnsafePointer,
    _ dataToSignLen: Int,
    _ sig: UnsafeMutablePointer,
    _ sigLen: UnsafeMutablePointer
) -> OSStatus
```

Deprecated

Use SecKeyCreateSignature

## Parameters 

`key`  

Private key with which to sign the data.

`padding`  

The type of padding to use. Possible values are listed in SecPadding. Use PKCS1SHA1 if the data to be signed is a SHA1 digest of the actual data. If you specify kSecPaddingNone, the data is signed as-is.

`dataToSign`  

The data to be signed. Typically, a digest of the actual data is signed.

`dataToSignLen`  

Length in bytes of the data in the `dataToSign` buffer. When PKCS1 padding is performed, the maximum length of data that can be signed is 11 bytes less than the value returned by the SecKeyGetBlockSize(_:) function (`secKeyGetBlockSize() - 11`).

`sig`  

On return, the digital signature.

`sigLen`  

On entry, the size of the buffer provided in the `sig` parameter. On return, the amount of data actually placed in the buffer.

## Return Value

A result code. See Security Framework Result Codes.

## Discussion

The behavior this function with kSecPaddingNone is undefined if the first byte of the data to sign is `0`; there is no way to verify leading zeroes, as they are discarded during the calculation.

