

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  passes() 

Instance Method

# passes()

Returns the passes in the user’s pass library that the app can access.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
func passes() -> [PKPass]
```

## Return Value

The passes in the user’s pass library.

## Discussion

Your app only has access to certain passes according to its entitlements. PassKit doesn’t return passes that your app can’t access.

Passes don’t have a fixed order. Calling this method multiple times may return the same passes, but in a different order.

## See Also

### Accessing passes

class func isPassLibraryAvailable() -> Bool

Returns a Boolean value that indicates whether the pass library is available.

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

