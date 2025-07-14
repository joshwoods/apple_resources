

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  serviceProviderData(for:completion:) 

Instance Method

# serviceProviderData(for:completion:)

Calls a completion handler that returns the custom data for a Secure Element pass.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.12+visionOS 1.0+watchOS 8.0+

``` source
func serviceProviderData(
    for secureElementPass: PKSecureElementPass,
    completion: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func serviceProviderData(for secureElementPass: PKSecureElementPass) async throws -> Data
```

## Parameters 

`secureElementPass`  

The Secure Element pass to check for secure data.

`completion`  

The completion block called by the system that returns the data or an error.

This block takes the following parameters:

`serviceProviderData`  
The custom data for the Secure Element pass; otherwise, null.

`error`  
If the process fails, an NSError that describes the failure; otherwise, null.

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

var remoteSecureElementPasses: [PKSecureElementPass]

The Secure Element passes that PassKit stores on paired devices.

