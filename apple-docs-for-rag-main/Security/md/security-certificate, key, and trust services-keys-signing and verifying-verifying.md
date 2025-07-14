

- Security
- Certificate, Key, and Trust Services
- Keys
-  Signing and Verifying 

Article

# Signing and Verifying

Create and evaluate digital signatures to establish the validity of code or data.

## Overview

You create a cryptographic signature on a block of data by first creating a hash of the data and then encrypting this digest with your private key. A recipient uses your public key to decrypt the signature, while independently re-creating the hash of the original data. If the decrypted hash and the computed one match, the recipient can be sure the data is from the owner of the private key that corresponds to the public key.

Often, you sign a block of data as a side effect of performing some other operation. For example, as a final step in distributing your app, Xcode signs the code on your behalf using one of your cryptographic identities (see Code Signing Guide). When you want to sign or verify a block of data in your app, you use functions provided by the certificate, key, and trust services API.

### Get Your Private Key

Begin by getting your private key, as described in Getting an Existing Key, either from the keychain or from an identity (which itself probably resides in the keychain). Then, select one of the signing algorithms. For example:

- Swift
- Objective-C

```
let privateKey: SecKey = 
let algorithm: SecKeyAlgorithm = .rsaSignatureMessagePKCS1v15SHA512
```

```
SecKeyRef privateKey = ;  // E.g., from the keychain
SecKeyAlgorithm algorithm = kSecKeyAlgorithmRSASignatureMessagePKCS1v15SHA512;
```

This algorithm indicates that the signing function should first create an SHA-512 digest of the input data and then use RSA encryption with PKCS#1 padding. But you can choose different options, along a number of dimensions:

- **Digest vs. message.** If you already have a digest of the data, you can use one of the `Digest` algorithms. For example, the above algorithm might become rsaSignatureDigestPKCS1v15SHA512. If you do this, be sure that the actual hashing matches the named hashing algorithm.

- **Digital signature algorithm type.** If you have elliptic curve keys instead of RSA, you can use an Elliptic Curve Digital Signature Algorithm (ECDSA). For example, the above algorithm might become ecdsaSignatureMessageX962SHA512.

With a key and an algorithm selected, you can test the compatibility of these with the signing operation using the SecKeyIsAlgorithmSupported(_:_:_:) function:

- Swift
- Objective-C

```
guard SecKeyIsAlgorithmSupported(privateKey, .sign, algorithm) else {
    throw 
}
```

```
BOOL canSign = SecKeyIsAlgorithmSupported(privateKey,
                                          kSecKeyOperationTypeSign,
                                          algorithm);
```

This function might return false, for example, if the key’s kSecAttrCanSign attribute is set to false. This situation might happen if you used a public key instead of a private one (despite the variable name). Similarly, if you attempt to use an RSA key with one of the ECDSA algorithms, the check fails.

Finally, you can create the signature with a call to the SecKeyCreateSignature(_:_:_:_:) function:

- Swift
- Objective-C

```
var error: Unmanaged?
guard let signature = SecKeyCreateSignature(privateKey,
                                            algorithm,
                                            data as CFData,
                                            &error) as Data? else {
                                                throw error!.takeRetainedValue() as Error
}
```

```
NSData* data2sign = ;
NSData* signature = nil;
if (canSign) {
    CFErrorRef error = NULL;
    signature = (NSData*)CFBridgingRelease(       // ARC takes ownership
                     SecKeyCreateSignature(privateKey,
                                           algorithm,
                                           (__bridge CFDataRef)data2sign,
                                           &error));
    if (!signature) {
        NSError *err = CFBridgingRelease(error);  // ARC takes ownership
        // Handle the error. . .
    }
}

```

If something goes wrong, the function returns a `nil` signature and populates the error reference with a doc://com.apple.documentation/documentation/corefoundation/cferror-ru8 object that explains the failure. In Objective-C, you transfer management of the error object, if it exists, to Automatic Reference Counting (ARC). In Swift, you transfer control of this unmanaged object’s memory to the system with a call to takeRetainedValue() and recast as an Error.

### Transmit the Data

After you successfully generate a signature, you transmit the data and signature to any interested party. Using your public key, the recipient then verifies the signature by performing a set of operations that resemble the signing process. As the receiver, you first retrieve the public key, possibly from a certificate, as described in Getting an Existing Key. Then, using the same algorithm as was used for signing, you test that the key and algorithm are mutually compatible with the verification operation:

- Swift
- Objective-C

```
guard SecKeyIsAlgorithmSupported(publicKey, .verify, algorithm) else {
    throw 
}
```

```
SecKeyRef publicKey = ;  // E.g., from a cert
BOOL canVerify = SecKeyIsAlgorithmSupported(publicKey,
                                            kSecKeyOperationTypeVerify,
                                            algorithm);
```

The SecKeyIsAlgorithmSupported(_:_:_:) function returns false if you use the wrong kind of key for the operation or algorithm. You then conduct the verification with a call to the SecKeyVerifySignature(_:_:_:_:_:) function:

- Swift
- Objective-C

```
var error: Unmanaged?
guard SecKeyVerifySignature(publicKey,
                            algorithm,
                            data as CFData,
                            signature as CFData,
                            &error) else {
                                throw error!.takeRetainedValue() as Error
}
```

```
BOOL result = NO;
if (canVerify) {
    CFErrorRef error = NULL;
    result = SecKeyVerifySignature(publicKey,
                                   algorithm,
                                   (__bridge CFDataRef)data2sign,
                                   (__bridge CFDataRef)signature,
                                   &error);
    if (!result) {
        NSError *err = CFBridgingRelease(error);  // ARC takes ownership
        // Handle the error. . .
    }
}

```

If the call succeeds and the signature and data are intact, the return value is true. If the function returns false, either the data or signature has been altered, the public key doesn’t match the private key, or some other error has occurred. Handle the error and transfer error object ownership to the system as needed.

