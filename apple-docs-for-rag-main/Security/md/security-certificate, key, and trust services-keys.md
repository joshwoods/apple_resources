

- Security
- Certificate, Key, and Trust Services
-  Keys 

API Collection

# Keys

Generate, store, and use cryptographic keys.

## Overview

Cryptographic keys are strings of bytes that you combine with other data in specialized mathematical operations to enhance security. At the lowest level, this usually means participating in either encryption and decryption or digital signing and verification. You can use these basic operations directly, such as when you encrypt data before sending it through an insecure channel. You also use them implicitly, such as when you verify the digital signature on a certificate as a byproduct of a trust evaluation.

Keys vary based on the operations they support. For example, you use public and private key pairs to perform asymmetric encryption, whereas you use symmetric keys to conduct symmetric encryption. Similarly, one key might work for a 1024-bit RSA algorithm, while another might be suitable for a 256-bit elliptic curve algorithm. Use the functions in this section when you need to handle cryptographic keys.

## Topics

### Essentials

Getting an Existing Key

Learn how to obtain an existing cryptographic key.

Storing Keys in the Keychain

Store and access cryptographic keys in the keychain.

class SecKey

An object that represents a cryptographic key.

func SecKeyGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which a key object belongs.

### Key Generation

Generating New Cryptographic Keys

Create both asymmetric and symmetric cryptographic keys.

Protecting keys with the Secure Enclave

Create an extra layer of security for your private keys.

func SecKeyCreateRandomKey(CFDictionary, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecKey?

Generates a new public-private key pair.

func SecKeyCopyPublicKey(SecKey) -> SecKey?

Gets the public key associated with the given private key.

Key Generation Attributes

Use attribute dictionary keys during cryptographic key generation.

### Examining Keys

func SecKeyIsAlgorithmSupported(SecKey, SecKeyOperationType, SecKeyAlgorithm) -> Bool

Returns a Boolean indicating whether a key is suitable for an operation using a certain algorithm.

func SecKeyGetBlockSize(SecKey) -> Int

Gets the block length associated with a cryptographic key.

func SecKeyCopyAttributes(SecKey) -> CFDictionary?

Gets the attributes of a given key.

struct SecKeyAlgorithm

The algorithms that cryptographic keys enable.

enum SecKeyOperationType

The types of operations that you can use a cryptographic key to perform.

### Import and Export

Storing Keys as Data

Create an external representation of a key for transmission.

func SecKeyCopyExternalRepresentation(SecKey, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFData?

Returns an external representation of the given key suitable for the key’s type.

func SecKeyCreateWithData(CFData, CFDictionary, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecKey?

Restores a key from an external representation of that key.

### Key Exchange

func SecKeyCopyKeyExchangeResult(SecKey, SecKeyAlgorithm, SecKey, CFDictionary, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFData?

Performs the Diffie-Hellman style of key exchange with optional key-derivation steps.

struct SecKeyKeyExchangeParameter

The dictionary keys used to specify Diffie-Hellman key exchange parameters.

### Encryption

Using Keys for Encryption

Perform asymmetric and symmetric encryption and decryption using cryptographic keys.

func SecKeyCreateEncryptedData(SecKey, SecKeyAlgorithm, CFData, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFData?

Encrypts a block of data using a public key and specified algorithm.

func SecKeyCreateDecryptedData(SecKey, SecKeyAlgorithm, CFData, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFData?

Decrypts a block of data using a private key and specified algorithm.

### Digital Signatures

Signing and Verifying

Create and evaluate digital signatures to establish the validity of code or data.

func SecKeyCreateSignature(SecKey, SecKeyAlgorithm, CFData, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFData?

Creates the cryptographic signature for a block of data using a private key and specified algorithm.

func SecKeyVerifySignature(SecKey, SecKeyAlgorithm, CFData, CFData, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

Verifies the cryptographic signature of a block of data using a public key and specified algorithm.

### Legacy iOS Key Operations

func SecKeyGeneratePair(CFDictionary, UnsafeMutablePointer&lt;SecKey?>?, UnsafeMutablePointer&lt;SecKey?>?) -> OSStatus

Creates an asymmetric key pair.

Deprecated

func SecKeyEncrypt(SecKey, SecPadding, UnsafePointer&lt;UInt8>, Int, UnsafeMutablePointer&lt;UInt8>, UnsafeMutablePointer&lt;Int>) -> OSStatus

Encrypts a block of plaintext.

Deprecated

func SecKeyDecrypt(SecKey, SecPadding, UnsafePointer&lt;UInt8>, Int, UnsafeMutablePointer&lt;UInt8>, UnsafeMutablePointer&lt;Int>) -> OSStatus

Decrypts a block of ciphertext.

Deprecated

func SecKeyRawSign(SecKey, SecPadding, UnsafePointer&lt;UInt8>, Int, UnsafeMutablePointer&lt;UInt8>, UnsafeMutablePointer&lt;Int>) -> OSStatus

Generates a digital signature for a block of data.

Deprecated

func SecKeyRawVerify(SecKey, SecPadding, UnsafePointer&lt;UInt8>, Int, UnsafePointer&lt;UInt8>, Int) -> OSStatus

Verifies a digital signature.

Deprecated

struct SecPadding

The types of padding to use when you create or verify a digital signature.

Deprecated

### Legacy macOS Key Operations

func SecKeyGeneratePairAsync(CFDictionary, dispatch_queue_t, SecKeyGeneratePairBlock)

Generates a public/private key pair.

Deprecated

func SecKeyGenerateSymmetric(CFDictionary, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecKey?

Generates a random symmetric key.

Deprecated

func SecKeyCreateFromData(CFDictionary, CFData, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecKey?

Constructs a SecKeyRef object for a symmetric key.

Deprecated

func SecKeyDeriveFromPassword(CFString, CFDictionary, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecKey?

Returns a key object in which the key data is derived from a password.

Deprecated

func SecKeyWrapSymmetric(SecKey, SecKey, CFDictionary, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFData?

Wraps a symmetric key with another key.

Deprecated

func SecKeyUnwrapSymmetric(UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>, SecKey, CFDictionary, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecKey?

Unwraps a wrapped symmetric key.

Deprecated

enum SecKeySizes

The supported sizes for keys of various common types.

Deprecated

struct SecKeyUsage

The flags that indicate key usage in the `KeyUsage` extension of a certificate.

typealias SecPublicKeyHash

A container for a 20-byte public key hash.

typealias SecKeyGeneratePairBlock

A block called with the results of a call to SecKeyGeneratePairAsync(_:_:_:).

enum SecCredentialType

The credential type to be returned by SecKeyGetCredentials.

Deprecated

