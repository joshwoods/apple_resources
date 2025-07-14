

- DeviceCheck
- DCAppAttestService
-  isSupported 

Instance Property

# isSupported

A Boolean value that indicates whether a particular device provides the App Attest service.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 15.0+visionOS 1.0+watchOS 9.0+

``` source
var isSupported: Bool { get }
```

## Mentioned in 

Establishing your app’s integrity

## Discussion

Important

Not all device types support the App Attest service, so check for support before using the service.

If you read isSupported from an app running on a Mac device, the value is false. This includes Mac Catalyst apps, and iOS or iPadOS apps running on Apple silicon.

If you read isSupported from within an app extension, the value might be true or false, depending on the extension type. However, most extensions don’t support App Attest. The generateKey(completionHandler:) method fails when you call it from an app extension, regardless of the value of isSupported.

The only app extensions that support App Attest are watchOS extensions in watchOS 9 or later. For these extensions, you can use the results from isSupported to indicate whether your WatchKit extension bypasses attestation.

## See Also

### Accessing the service

class var shared: DCAppAttestService

The shared App Attest service that you use to validate your app.

