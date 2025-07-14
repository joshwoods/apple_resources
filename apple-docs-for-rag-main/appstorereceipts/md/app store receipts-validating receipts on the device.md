

- App Store Receipts
-  Validating receipts on the device 

Article

# Validating receipts on the device

Verify the contents of app receipts by decoding and parsing the receipt on the device.

## Overview

When users install apps from the App Store, the app contains a cryptographically signed receipt that Apple creates and stores inside the app bundle, which you can then validate.

Note

The receipt isn’t necessary if you use AppTransaction to validate the app download, or Transaction to validate in-app purchases. Only use the receipt if your app uses the Original API for In-App Purchase, or needs the receipt to validate the app download because it can’t use `AppTransaction`.

Validating the receipt locally requires you to develop or use code to read and decode the receipt as a PKCS #7 container, as defined by RFC 2315. The App Store encodes the payload of the container using Abstract Syntax Notation One (ASN.1), as defined by ITU-T X.690. The payload contains a set of receipt attributes. Each receipt attribute contains a type, a version, and a value.

The App Store defines the structure of the payload with the following ASN.1 notation:

ReceiptModule DEFINITIONS ::=
BEGIN

ReceiptAttribute ::= SEQUENCE {
    type    INTEGER,
    version INTEGER,
    value   OCTET STRING
}

Payload ::= SET OF ReceiptAttribute

END

### Validate the receipt

In macOS and Mac apps built with Mac Catalyst, implement receipt validation in the main function, before the app calls NSApplicationMain(_:_:).

To validate the app receipt, perform the following tests in order:

1.  Locate and load the app receipt from the app’s bundle. The class Bundle provides the location of the receipt with the property appStoreReceiptURL.

2.  Decode the app receipt as a PKCS #7 container and verify that the chain of trust for the container’s signature traces back to the Apple Inc. Root certificate, available from Apple PKI. Use the `receipt_creation_date`, identified as ASN.1 Field Type 12 when validating the receipt signature.

3.  Verify that the bundle identifier, identified as ASN.1 Field Type 2, matches your app’s bundle identifier.

4.  Verify that the version identifier string, identified as ASN.1 Field Type 3, matches the version string in your app’s bundle.

5.  Compute a SHA-1 hash for the device that installs the app and verify that it matches the receipt’s hash, identified as ASN.1 Field Type 5.

The validation passes if all of the tests pass. If any test fails, the validation fails.

For information about the keys in a receipt, see Receipt Fields.

### Verify the certificate chain of trust

Decode the app receipt as a PKCS #7 container and verify that the chain of trust for the container’s signature traces back to the Apple Inc. Root certificate, available from Apple PKI.

Tip

Don’t hardcode intermediate certificates in your app. Ensure that your code supports certificates that use SHA-256 and SHA-1 signing algorithms.

Make sure your app uses the date from the `receipt_creation_date` field, identified as ASN.1 Field Type 12, to validate the receipt’s signature. Many cryptographic libraries default to using the device’s current time and date when validating a PKCS \#7 package, but this may not produce the correct results when validating a receipt’s signature. For example, if the receipt was signed with a valid certificate, but the certificate has since expired, using the device’s current date incorrectly returns an invalid result.

### Compute the SHA-1 hash

Compute the SHA-1 hash to match the local device with the device hash inside the App Store reciept. When computing the SHA-1 hash, use the platform-specific data source. The source of bytes for each platform is:

- watchOS: Use the raw bytes from the uuid property of the UUID that identifierForVendor provides.

- iOS, iPadOS, tvOS, and iOS apps running on a Mac with Apple silicon: Use the raw bytes from the uuid property of the UUID that identifierForVendor provides.

- macOS and apps built with Mac Catalyst: Use the data that returns from `copy_mac_address` from the example code below.

The following two code examples illustrate how to retrieve an identifier in macOS, as the `copy_mac_address` function shows, for validating an App Store receipt.

In the following Swift code, the `io_service` function uses IOKit to retrieve network interfaces as an optional IOKit object. The `copy_mac_address` function looks up an appropriate network interface and returns the hardware address from the IOKit object as optional `CFData`.

The following Objective-C code works in the same fashion. This example uses IOKit to look up the relevant network interface, and returns the bytes that identify the built-in network interface:

### Respond to validation failures

If your app receipt validation fails, respond to that failure as follows:

- Don’t try to terminate the app. Without a validated receipt, assume the user doesn’t have access to premium content. Provide a user interface to gracefully handle this case and inform the user what they can do to get full access to your app’s features.

- If the app receipt is missing or corrupt, use the SKReceiptRefreshRequest object to refresh the app receipt.

- In the sandbox environment, if the app receipt is missing, assume the tester is a new customer and doesn’t have access to premium content.

Note

For apps in iOS and iPadOS running in the sandbox environment and in StoreKit testing in Xcode, the app receipt is present only after the tester makes their first in-app purchase. The app receipt is always present in TestFlight on devices running macOS.

