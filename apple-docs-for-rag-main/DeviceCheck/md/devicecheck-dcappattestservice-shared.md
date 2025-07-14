

- DeviceCheck
- DCAppAttestService
-  shared 

Type Property

# shared

The shared App Attest service that you use to validate your app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 15.0+visionOS 1.0+watchOS 9.0+

``` source
class var shared: DCAppAttestService { get }
```

## Mentioned in 

Establishing your app’s integrity

Validating apps that connect to your server

## Discussion

Use the shared instance of the service to generate and to certify a cryptographic key, and then to assert your app’s validity using that key.

## See Also

### Accessing the service

var isSupported: Bool

A Boolean value that indicates whether a particular device provides the App Attest service.

