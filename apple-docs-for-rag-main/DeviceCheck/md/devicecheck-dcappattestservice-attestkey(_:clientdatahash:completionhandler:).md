

- DeviceCheck
- DCAppAttestService
-  attestKey(\_:clientDataHash:completionHandler:) 

Instance Method

# attestKey(\_:clientDataHash:completionHandler:)

Asks Apple to attest to the validity of a generated cryptographic key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 15.0+visionOS 1.0+watchOS 9.0+

``` source
func attestKey(
    _ keyId: String,
    clientDataHash: Data,
    completionHandler: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func attestKey(
    _ keyId: String,
    clientDataHash: Data
) async throws -> Data
```

## Parameters 

`keyId`  

The identifier you received when generating a cryptographic key by calling the generateKey(completionHandler:) method.

`clientDataHash`  

A SHA256 hash of a unique, single-use data block that embeds a challenge from your server. Should be at least 16 bytes in length.

`completionHandler`  

A closure that the method calls upon completion with the following parameters:

- `attestationObject`: A statement from Apple about the validity of the key associated with `keyId`. Send this to your server for processing.

- `error`: A DCError instance that indicates the reason for failure, or `nil` on success.

## Mentioned in 

Preparing to use the app attest service

Establishing your app’s integrity

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method asks Apple to attest to the validity of a key that you previously generated with a call to the generateKey(completionHandler:) method. Provide the method with both the key identifier and a computed hash of a data block that includes a one-time challenge from your server to prevent replay attacks. For example, you can use CryptoKit to create a SHA256 hash of challenge data:

```
```

The attest method calls its completion handler to return an attestation object to you, which you must send to your server for verification. A compromised version of your app could falsify the verification result, thus circumventing App Attest.

If you successfully verify the attestation object on your server, as described in Validating apps that connect to your server, then you can associate the key identifier with the user on the device for future reference. You’ll need the identifier to generate assertions with calls to generateAssertion(_:clientDataHash:completionHandler:). If your server fails to verify the attestation object, discard the key identifier.

If the method’s completion handler returns the serverUnavailable error — typically due to network connectivity issues — it means that the framework failed to reach the App Attest service to complete the attestation. In this case, retry attestation again using the same key and client data hash later to avoid unnecessarily generating new keys. Retrying with the same inputs helps to preserve the risk metric for a given device.

## See Also

### Preparing a key

func generateKey(completionHandler: (String?, (any Error)?) -> Void)

Creates a new cryptographic key for use with the App Attest service.

