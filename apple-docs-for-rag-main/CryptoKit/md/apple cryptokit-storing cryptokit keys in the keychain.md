

- Apple CryptoKit
-  Storing CryptoKit Keys in the Keychain 

Sample Code

# Storing CryptoKit Keys in the Keychain

Convert between strongly typed cryptographic keys and native keychain types.

Download

iOS 13.0+iPadOS 13.0+macOS 10.15+Xcode 11.0+

## Overview

CryptoKit defines highly specific key types that embody a particular cryptographic algorithm and purpose. Some of these key types, like P256.Signing.PrivateKey, correspond to items that the Keychain services API stores natively as SecKey instances. Other key types, like Curve25519.Signing.PrivateKey, have no direct keychain corollary. To store these kinds of keys, you package them as generic passwords.

This sample code project demonstrates the conversions needed to store all the CryptoKit key types in the keychain.

### Configure the Sample Code Project

The sample provides targets for both iOS and macOS. For both platforms, specify your developer team in the Xcode Signing & Capabilities tab before building. The macOS target also sets the Keychain Access Groups Entitlement, to enable access to the keychain on that platform.

### Declare the Convertibility of NIST Keys

Keychain services lets you convert between SecKey instances and data in the X9.63 data format. For NIST keys that support that representation, like P256, P384, and P521, CryptoKit defines a property that you use to get the X9.63 data. The framework also provides a complementary initializer that creates a new key from data in that format.

Define a protocol called `SecKeyConvertible` to express this interface:

Then assert that all the NIST private keys adopt this protocol:

### Declare the Convertibility of Other Key Types

Keychain services also lets you securely store small chunks of data as a generic password keychain item. For any CryptoKit key without a X9.63 representation, CryptoKit provides a means to obtain a data representation of the key, enabling generic password storage. Define the `GenericPasswordConvertible` protocol to establish an interface for these items:

Some keys, like Curve25519, adopt this interface directly, and you simply assert that they do:

Other keys offer similar functionality, but require modest adjustments to their interface. For example, you provide a secure conversion for instances of SymmetricKey:

Keys that you store in the Secure Enclave expose a raw representation as well, but in this case the data isn’t the raw key. Instead, the Secure Enclave exports an encrypted block that only the same Secure Enclave can later use to restore the key. You can adopt the same convertibility protocol to store the Secure Enclave’s encrypted data in the keychain as a generic password, and later allow the Secure Enclave to reconstruct the key on the same device:

### Store a NIST Key

To store a NIST key in the keychain, create a storage method that constrains input keys to be of type `SecKeyConvertible`:

Then call the SecKeyCreateWithData(_:_:_:) function with the X9.63 representation of the key to create a SecKey instance. Include attributes that describe the key as a private, elliptic-curve key.

Store the SecKey representation in the keychain by placing it in an add query and calling the SecItemAdd(_:_:) function. Give the key a label to make it easier to find later.

### Store Other Key Types in the Keychain

To store other kinds of keys, create a different storage method that constrains input keys to be of type `GenericPasswordConvertible`:

In this case, you provide the raw representation as the data for the password item, and store that with a call to the SecItemAdd(_:_:) function:

### Retrieve a NIST Key as a Native Keychain Key

You retrieve a key from the keychain using a call to the SecItemCopyMatching(_:_:) function. Construct a query dictionary that pinpoints the particular key that you want to find. After your search returns the desired key—stored as a SecKeychainItem instance—you cast it as a SecKey instance.

Note

The above query returns the first elliptic-curve key with the given label found in the user’s keychain. You might need to perform a more sophisticated search if more than one key might match, as described in Storing Keys in the Keychain.

After you get the SecKey reference, initialize a CryptoKit key using the X9.63 representation returned by the SecKeyCopyExternalRepresentation(_:_:) function.

Make sure that the type of the key that you initialize using the data matches the type of the original key. For example, initializing a P256 key from the data corresponding to a keychain item that you created using a P384 key produces undefined results.

### Retrieve Keys Stored as Generic Passwords

You also retrieve generic passwords using the SecItemCopyMatching(_:_:) function, in this case using kSecClassGenericPassword for the item’s class. You convert the returned item to data, and use it directly to instantiate a key of the corresponding type:

As long as the type you initialize matches the type that you previously used to store the item in the keychain, the initialization correctly reconstructs the key.

