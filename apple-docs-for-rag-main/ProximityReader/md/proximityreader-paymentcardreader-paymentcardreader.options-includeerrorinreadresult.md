

- ProximityReader
- PaymentCardReader
- PaymentCardReader.Options
-  includeErrorInReadResult 

Instance Property

# includeErrorInReadResult

A Boolean value that indicates whether the framework returns a result instead of throwing an error when some data is retrievable.

iOS 16.4+iPadOS 16.4+Mac Catalyst 17.0+

``` source
var includeErrorInReadResult: Bool
```

## Discussion

The default value is `false`.

After the framework reads a payment card, when there’s an error, the framework discards PaymentCardReadResult and throws an error.

When you set this option to `true`, if an error arises, the framework doesn’t throw an error, instead the PaymentCardReadResult includes both the outcome and the data that the framework can retrieve. You’re responsible for checking the outcome in addition to catching errors the framework throws.

## See Also

### Setting read behaviors

var returnReadResultImmediately: Bool

A Boolean value that indicates whether the framework returns a result as soon as possible before closing the system UI.

