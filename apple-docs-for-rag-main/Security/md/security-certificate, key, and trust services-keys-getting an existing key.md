

- Security
- Certificate, Key, and Trust Services
- Keys
-  Getting an Existing Key 

Article

# Getting an Existing Key

Learn how to obtain an existing cryptographic key.

## Overview

The Security framework defines the SecKey opaque type to hold key objects. You typically use a key reference to indicate the key to use for a particular cryptographic operation, such as encryption. How you get a key reference depends on where the key is stored. In particular, the source of a key might be one of the following:

- **An identity.** When you read an identity from a password-protected file or from the keychain, you can extract the private key it contains, as described in Parsing an Identity. In macOS, you can also store a private key in an identity, along with its certificate, as described in Creating an Identity.

- **A trust.** When you have a trust object, as described in Evaluating a Trust and Parsing the Result, you can extract the associated certificate’s public key with a call to SecTrustCopyPublicKey(_:):

- Swift
- Objective-C

```
  let publicKey = SecTrustCopyPublicKey(trust)
```

```
  SecKeyRef publicKey = SecTrustCopyPublicKey(trust);
```

- **Another key.** When you have a private key, you can calculate the associated public key with the SecKeyCopyPublicKey(_:) function:

- Swift
- Objective-C

```
  let publicKey = SecKeyCopyPublicKey(privateKey)
```

```
  SecKeyRef publicKey = SecKeyCopyPublicKey(privateKey);
```

- **Data.** You can export a key as a data blob that you can store on disk or send to someone else. Your app or another process can then do the reverse and restore the key from the data, possibly at a later time. See Storing Keys as Data for more details.

- **The keychain.** You can place a key in a keychain to securely store it for later use. See Storing Keys in the Keychain for more details.

