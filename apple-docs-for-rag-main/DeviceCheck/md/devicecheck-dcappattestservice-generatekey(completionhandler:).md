

- DeviceCheck
- DCAppAttestService
-  generateKey(completionHandler:) 

Instance Method

# generateKey(completionHandler:)

Creates a new cryptographic key for use with the App Attest service.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 15.0+visionOS 1.0+watchOS 9.0+

``` source
func generateKey(completionHandler: @escaping (String?, (any Error)?) -> Void)
```

``` source
func generateKey() async throws -> String
```

## Parameters 

`completionHandler`  

A closure that the method calls upon completion with the following parameters:

- `keyId`: An identifier that you use to refer to the key. The framework securely stores the key in the Secure Enclave.

- `error`: A DCError instance that indicates the reason for failure, or `nil` on success.

## Mentioned in 

Establishing your app’s integrity

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func generateKey() async throws -> String
```

For example:

```
let keyIdentifier = try await generateKey()
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Call this method to request the creation of a secure, unattested key pair on a device for a specific user. On success, the method provides your app with an identifier that represents the key pair stored in the Secure Enclave. Because there’s no way to use or retrieve the key without the identifier, you’ll want to either record it in your app or on your server right away. If key generation fails, the closure provides a DCError that indicates the reason for the failure.

Create a unique key for each user account on a device. Otherwise it’s hard to detect an attack that uses a single compromised device to serve multiple remote users running a compromised version of your app. For more information, see Assessing fraud risk.

After you get the identifier, you call the attestKey(_:clientDataHash:completionHandler:) method with the key identifier to ask Apple to attest to the validity of the associated key. Later, you call the generateAssertion(_:clientDataHash:completionHandler:) method with the key identifier to answer a challenge from your server, and establish the legitimacy of this instance of your app.

## See Also

### Preparing a key

func attestKey(String, clientDataHash: Data, completionHandler: (Data?, (any Error)?) -> Void)

Asks Apple to attest to the validity of a generated cryptographic key.

