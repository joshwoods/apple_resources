

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  containsPass(\_:) 

Instance Method

# containsPass(\_:)

Returns a Boolean value that indicates whether the user’s pass library contains the specified pass.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
func containsPass(_ pass: PKPass) -> Bool
```

## Parameters 

`pass`  

The pass to query.

## Return Value

true if the user’s pass library contains the pass; otherwise, false.

## Discussion

This method lets you determine that the pass library contains a pass even though your app can’t read or modify the pass. For example, an email client doesn’t have entitlements to read or write any passes from the library.

Your app can use this method to provide a UI that indicates whether a pass is already in the library.

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

func serviceProviderData(for: PKSecureElementPass, completion: (Data?, (any Error)?) -> Void)

Calls a completion handler that returns the custom data for a Secure Element pass.

var remoteSecureElementPasses: [PKSecureElementPass]

The Secure Element passes that PassKit stores on paired devices.

