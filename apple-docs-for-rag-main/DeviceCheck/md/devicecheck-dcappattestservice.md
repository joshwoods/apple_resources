

- DeviceCheck
-  DCAppAttestService 

Class

# DCAppAttestService

A service that you use to validate the instance of your app running on a device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 15.0+visionOS 1.0+watchOS 9.0+

``` source
class DCAppAttestService
```

## Mentioned in 

Establishing your app’s integrity

Validating apps that connect to your server

## Overview

Use the shared instance of the DCAppAttestService class to assert the legitimacy of a particular instance of your app to your server. After ensuring service availability by reading the isSupported property, you use the service to:

- Create a cryptographic key in the Secure Enclave by calling the generateKey(completionHandler:) method.

- Ask Apple to certify the key by calling the attestKey(_:clientDataHash:completionHandler:) method. - Prepare an assertion of your app’s integrity to accompany any or all server requests using the generateAssertion(_:clientDataHash:completionHandler:) method.

For more information about how to support App Attest in your app, see Establishing your app’s integrity. For information about the complementary procedures you implement on your server, see Validating apps that connect to your server.

Note

To use the App Attest service, your app must have an app ID that you register on the Apple Developer website.

## Topics

### Accessing the service

class var shared: DCAppAttestService

The shared App Attest service that you use to validate your app.

var isSupported: Bool

A Boolean value that indicates whether a particular device provides the App Attest service.

### Preparing a key

func generateKey(completionHandler: (String?, (any Error)?) -> Void)

Creates a new cryptographic key for use with the App Attest service.

func attestKey(String, clientDataHash: Data, completionHandler: (Data?, (any Error)?) -> Void)

Asks Apple to attest to the validity of a generated cryptographic key.

### Validating the app instance

func generateAssertion(String, clientDataHash: Data, completionHandler: (Data?, (any Error)?) -> Void)

Creates a block of data that demonstrates the legitimacy of an instance of your app running on a device.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### App Attest

Establishing your app’s integrity

Ensure that requests your server receives come from legitimate instances of your app.

Validating apps that connect to your server

Verify that connections to your server come from legitimate instances of your app.

Assessing fraud risk

Request and analyze risk data using server-to-server calls.

Preparing to use the app attest service

Test your implementation in a development environment and onboard users gradually.

App Attest Environment

The environment for an app that uses the App Attest service to validate itself.

