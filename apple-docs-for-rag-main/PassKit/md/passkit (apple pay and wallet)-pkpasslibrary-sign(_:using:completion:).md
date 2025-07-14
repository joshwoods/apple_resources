

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  sign(\_:using:completion:) 

Instance Method

# sign(\_:using:completion:)

Signs an opaque value using a cryptographic signature.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.12+visionOS 1.0+watchOS 6.2+

``` source
func sign(
    _ signData: Data,
    using secureElementPass: PKSecureElementPass,
    completion: @escaping (Data?, Data?, (any Error)?) -> Void
)
```

``` source
func sign(
    _ signData: Data,
    using secureElementPass: PKSecureElementPass
) async throws -> (Data, Data)
```

## Parameters 

`signData`  

The opaque value to sign.

`secureElementPass`  

The Secure Element pass that PassKit uses to generate the signature.

`completion`  

A Swift closure or an Objective-C block that PassKit runs when the process finishes.

`signedData`  
The signed value.

`signature`  
The cryptographic signature that PassKit uses to sign the value.

`error`  
If the process fails, an error that describes the failure; otherwise, `nil` in Swift or null in Objective-C.

## Discussion

Important

The method is available only to developers who work with Apple to enable this functionality.

PassKit may execute the completion Swift closure or an Objective-C block on an arbitrary queue.

