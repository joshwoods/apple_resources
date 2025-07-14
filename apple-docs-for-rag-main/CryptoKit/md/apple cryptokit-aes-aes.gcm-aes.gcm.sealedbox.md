

- Apple CryptoKit
- AES
- AES.GCM
-  AES.GCM.SealedBox 

Structure

# AES.GCM.SealedBox

A secure container for your data that you can access using a cipher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct SealedBox
```

## Overview

Use a sealed box as a container for data that you want to transmit securely. Seal data into a box with one of the cipher algorithms, like seal(_:using:nonce:).

The box holds an encrypted version of the original data, an authentication tag, and the nonce during encryption. The encryption makes the data unintelligible to anyone without the key, while the authentication tag makes it possible for the intended receiver to be sure the data remains intact.

The receiver uses another instance of the same cipher, like the open(_:using:) method, to open the box.

## Topics

### Creating the sealed box

init&lt;C, T>(nonce: AES.GCM.Nonce, ciphertext: C, tag: T) throws

Creates a sealed box from the given tag, nonce, and ciphertext.

init&lt;D>(combined: D) throws

Creates a sealed box from the combined bytes of an authentication tag, nonce, and encrypted data.

### Retrieving the combined contents

var combined: Data?

A combined element composed of the nonce, encrypted data, and authentication tag.

### Inspecting the component elements

var nonce: AES.GCM.Nonce

The nonce used to encrypt the data.

var ciphertext: Data

The encrypted data.

var tag: Data

An authentication tag.

## Relationships

### Conforms To

- Sendable

