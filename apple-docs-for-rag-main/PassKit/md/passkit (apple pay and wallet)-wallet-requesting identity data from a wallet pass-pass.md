

- PassKit (Apple Pay and Wallet)
- Wallet
-  Requesting identity data from a Wallet pass 

Article

# Requesting identity data from a Wallet pass

Initiate a request for identity information by prompting a user for permission and decrypting a response payload.

## Overview

The Wallet app allows people to store a state identification card, mobile driver’s license (mDL), or national identification card from a government issuing authority, such as the department of motor vehicles. These documents are between a person and the issuing authority — Apple doesn’t create or see the documents.

Beginning on iPhone with iOS 16, you can request information from IDs in Wallet to verify a person’s age or identity. If a person accepts the request, the system gets the information from their issuing authority and your app receives a payload. After decryption, the payload contains data that follows the ISO 18013-5 specification. To use the elements your app requests, send the payload to your server for verification.

For design guidance, see Human Interface Guidelines > Technologies > Wallet.

Important

This API only works on iPhone and returns an error if you access it on iPad. It requires a special entitlement from Apple. Building an app with this entitlement requires macOS 13 or later. For more information about the entitlement, see Getting started with the Verify with Wallet API.

### Create an identity document descriptor

Before you request information from an ID in Wallet, you create an object to describe the elements you need. Your app can only request the elements your entitlement grants. Create a PKIdentityDriversLicenseDescriptor if you’re requesting information from a person’s state or mobile driver’s license. Create a PKIdentityNationalIDCardDescriptor if you’re requesting information from their national identificaton card, and add the elements to the request.

For each element, you specify your intent to store the resulting data by using mayStore(days:), mayStore, or willNotStore. Upon request, the system presents the information for a person to review in a system sheet.

The framework allows for requesting the Boolean age(atLeast:) element for any age between `1` and `125` only if the issuer includes it. If an app requests age(atLeast:) and the `age_over_XX` element isn’t present in the mobile driver’s license, the framework falls back to a request for the age element.

An app can’t include both an age(atLeast:) element and an age element in the same request.

The following code shows the creation of PKIdentityDriversLicenseDescriptor requesting information from a person’s state or mobile driver’s license and PKIdentityNationalIDCardDescriptor requesting information from a person’s national identification card.

```
let driversLicenseDescriptor = PKIdentityDriversLicenseDescriptor()
driversLicenseDescriptor.addElements([.age(atLeast: 18)],
                       intentToStore: .willNotStore)
driversLicenseDescriptor.addElements([.givenName, 
                        .familyName,
                        .portrait],
                       intentToStore: .mayStore(days: 30))
```

```
let nationalIDCardDescriptor = PKIdentityNationalIDCardDescriptor()
nationalIDCardDescriptor.addElements([.age(atLeast: 18)],
                       intentToStore: .willNotStore)
nationalIDCardDescriptor.addElements([.givenName, 
                        .familyName,
                        .portrait],
                       intentToStore: .mayStore(days: 30))
```

To check whether the identity document you describe is available to request, create a PKIdentityAuthorizationController and call checkCanRequestDocument(_:completion:). If the document exists, show a PKIdentityButton to allow the user to begin the authorization request.

```
let controller = PKIdentityAuthorizationController()
controller.checkCanRequestDocument(descriptor) { canRequest in
    // Show or hide the identity button.
}
```

### Create a request

To create an identity request, you need the merchant identifier you configure in the developer portal. A merchant identifier never expires, and you can use the same one that you use for Apple Pay.

A request also needs a nonce to prevent your server from using a response document more than once. Your server needs the nonce to decrypt the response document, so generate it there and associate it with the user’s session.

```
let request = PKIdentityRequest()
request.descriptor = descriptor
request.merchantIdentifier = // The merchant identifier.
request.nonce = // The nonce your server generates.
```

Your app’s `Info.plist` file needs to provide a message for the `NSIdentityUsageDescription` key. If this key is missing, any attempt to request a document fails.

### Request the document

When requesting a document, the system presents a sheet to the user to confirm the request before retrieving any data. If the user rejects the request, your app receives a PKIdentityError.Code.cancelled error.

```
do {
    let document = try await controller.requestDocument(request)
} catch {
    // Handle the error.
}
```

When you receive a PKIdentityDocument, you’re ready to verify the request payload. The data in the encryptedData property isn’t readable on the device, so you need to send it to your server for verification.

The elements in PKIdentityDriversLicenseDescriptor map to a set of elements in the ISO and American Association of Motor Vehicle Administrators (AAMVA) namespaces in the response. For PKIdentityNationalIDCardDescriptor, the elements map to a set of elements in the ISO and JP namespace in the response. For a list of elements, see PKIdentityDriversLicenseDescriptor and PKIdentityNationalIDCardDescriptor.

Note

Only one request can be in progress at a time. Otherwise, the system returns a PKIdentityError.Code.requestAlreadyInProgress error.

To learn more about verifying identity requests, see Verifying Wallet identity requests.

### Test the implementation

Even if you don’t live in an area that supports IDs in Wallet, you can test your implementation through the iPhone simulator or by downloading a developer profile on your local device. When you request a document, you receive a mock mDL that’s similar to a real ID. When you test with the simulator, the response doesn’t include a real issuing authority or device signature. The developer test profile produces a real device signature, but not a real issuer signature. A mock mDL isn’t visible in the Wallet app, so don’t treat it as real. To activate a mock mDL on your device, download the Wallet identity developer profile from Profiles and Logs.

## See Also

### Identity sheet interactions and authorization

Verifying Wallet identity requests

Decrypt and verify an in-app presentment request on your server.

class PKIdentityAuthorizationController

An object that presents a sheet that prompts the user to allow a request for identity information.

class PKIdentityRequest

An object that represents a request for identity information from a Wallet pass.

class PKIdentityDocument

An object that represents the response to a request.

class PKIdentityElement

An object that represents the elements an app requests from identity documents.

class PKIdentityButton

An object that displays a button to trigger the identity verification flow.

struct VerifyIdentityWithWalletButton

A view that displays a button for identity verification.

struct VerifyIdentityWithWalletButtonLabel

A type that represents the label you use with a verify identity button.

struct VerifyIdentityWithWalletButtonStyle

A type that represents the style you use with a verify identity button.

