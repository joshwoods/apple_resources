

- Security
-  SecKeyRawVerify(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# SecKeyRawVerify(\_:\_:\_:\_:\_:\_:)

Verifies a digital signature.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedtvOS 4.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–8.0Deprecated

``` source
func SecKeyRawVerify(
    _ key: SecKey,
    _ padding: SecPadding,
    _ signedData: UnsafePointer,
    _ signedDataLen: Int,
    _ sig: UnsafePointer,
    _ sigLen: Int
) -> OSStatus
```

Deprecated

Use SecKeyVerifySignature

## Parameters 

`key`  

Public key with which to verify the data.

`padding`  

The type of padding used. Possible values are listed in SecPadding. Use PKCS1SHA1 if you are verifying a PKCS1-style signature with DER encoding of the digest type and the signed data is a SHA1 digest of the actual data. Specify kSecPaddingNone if no padding was used.

`signedData`  

The data for which the signature is being verified. Typically, a digest of the actual data is signed.

`signedDataLen`  

Length in bytes of the data in the `signedData` buffer.

`sig`  

The digital signature to be verified.

`sigLen`  

Length of the data in the `sig` buffer.

## Return Value

A result code. See Security Framework Result Codes.

