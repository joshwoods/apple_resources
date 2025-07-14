

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  passes(of:) 

Instance Method

# passes(of:)

Returns the passes of the specified pass type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 3.0+

``` source
func passes(of passType: PKPassType) -> [PKPass]
```

## Parameters 

`passType`  

One of the pass types in PKPassType.

## Return Value

An array of passes of the specified type.

## See Also

### Accessing passes

class func isPassLibraryAvailable() -> Bool

Returns a Boolean value that indicates whether the pass library is available.

func passes() -> [PKPass]

Returns the passes in the user’s pass library that the app can access.

func pass(withPassTypeIdentifier: String, serialNumber: String) -> PKPass?

Returns the pass with the specified pass type identifier and serial number.

func containsPass(PKPass) -> Bool

Returns a Boolean value that indicates whether the user’s pass library contains the specified pass.

func serviceProviderData(for: PKSecureElementPass, completion: (Data?, (any Error)?) -> Void)

Calls a completion handler that returns the custom data for a Secure Element pass.

var remoteSecureElementPasses: [PKSecureElementPass]

The Secure Element passes that PassKit stores on paired devices.

