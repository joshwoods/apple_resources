

- CryptoTokenKit
- TKTokenSmartCardPINAuthOperation
-  pin 

Instance Property

# pin

The PIN value resulting from performing the operation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var pin: String? { get set }
```

## Discussion

This property is set to the result of the operation after `finishWithError:` is called.

Note

If the apduTemplate property has a set value, this property is not set, as the PIN is automatically sent to the Smart Card using the specified template.

