

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassViewController
-  canAddSecureElementPass(configuration:) 

Type Method

# canAddSecureElementPass(configuration:)

Returns a Boolean value that indicates whether PassKit can create a Secure Element pass using the specified configuration.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
class func canAddSecureElementPass(configuration: PKAddSecureElementPassConfiguration) -> Bool
```

## Parameters 

`configuration`  

The configuration to validate.

## Return Value

true if PassKit validates the configuration; otherwise, false.

