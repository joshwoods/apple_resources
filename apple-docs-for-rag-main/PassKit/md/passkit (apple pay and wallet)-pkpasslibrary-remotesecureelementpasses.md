

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  remoteSecureElementPasses 

Instance Property

# remoteSecureElementPasses

The Secure Element passes that PassKit stores on paired devices.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.12+visionOS 1.0+watchOS 6.2+

``` source
var remoteSecureElementPasses: [PKSecureElementPass] { get }
```

## Discussion

This is an array that contains the Secure Element passes from all of the device’s remote paired devices, such as an Apple Watch.

## See Also

### Accessing passes

class func isPassLibraryAvailable() -> Bool

Returns a Boolean value that indicates whether the pass library is available.

func passes() -> [PKPass]

Returns the passes in the user’s pass library that the app can access.

func passes(of: PKPassType) -> [PKPass]

Returns the passes of the specified pass type.

func pass(withPassTypeIdentifier: String, serialNumber: String) -> PKPass?

Returns the pass with the specified pass type identifier and serial number.

func containsPass(PKPass) -> Bool

Returns a Boolean value that indicates whether the user’s pass library contains the specified pass.

func serviceProviderData(for: PKSecureElementPass, completion: (Data?, (any Error)?) -> Void)

Calls a completion handler that returns the custom data for a Secure Element pass.

