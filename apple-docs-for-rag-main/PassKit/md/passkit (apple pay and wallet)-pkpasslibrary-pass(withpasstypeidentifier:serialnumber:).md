

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  pass(withPassTypeIdentifier:serialNumber:) 

Instance Method

# pass(withPassTypeIdentifier:serialNumber:)

Returns the pass with the specified pass type identifier and serial number.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
func pass(
    withPassTypeIdentifier identifier: String,
    serialNumber: String
) -> PKPass?
```

## Parameters 

`identifier`  

The pass’s pass type identifier.

`serialNumber`  

The pass’s serial number.

## Return Value

The pass with the specified pass type identifier and serial number, or `nil` if there isn’t such a pass or if the app doesn’t have the appropriate entitlement.

## See Also

### Accessing passes

class func isPassLibraryAvailable() -> Bool

Returns a Boolean value that indicates whether the pass library is available.

func passes() -> [PKPass]

Returns the passes in the user’s pass library that the app can access.

func passes(of: PKPassType) -> [PKPass]

Returns the passes of the specified pass type.

func containsPass(PKPass) -> Bool

Returns a Boolean value that indicates whether the user’s pass library contains the specified pass.

func serviceProviderData(for: PKSecureElementPass, completion: (Data?, (any Error)?) -> Void)

Calls a completion handler that returns the custom data for a Secure Element pass.

var remoteSecureElementPasses: [PKSecureElementPass]

The Secure Element passes that PassKit stores on paired devices.

