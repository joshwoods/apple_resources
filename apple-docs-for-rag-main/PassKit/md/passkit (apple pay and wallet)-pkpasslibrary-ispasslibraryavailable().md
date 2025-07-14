

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  isPassLibraryAvailable() 

Type Method

# isPassLibraryAvailable()

Returns a Boolean value that indicates whether the pass library is available.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
class func isPassLibraryAvailable() -> Bool
```

## Return Value

true if the pass library is available; otherwise, false.

## Discussion

This method exists because the pass library may be unavailable even if the PKPassLibrary class exists.

Note

Don’t use this method to determine whether the user can add passes on the device. A device may have a pass library, but still not be able to add passes. Use the PKAddPassesViewController class’s canAddPasses() method instead.

## See Also

### Accessing passes

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

var remoteSecureElementPasses: [PKSecureElementPass]

The Secure Element passes that PassKit stores on paired devices.

