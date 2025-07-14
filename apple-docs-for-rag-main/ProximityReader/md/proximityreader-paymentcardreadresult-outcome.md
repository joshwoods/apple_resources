

- ProximityReader
- PaymentCardReadResult
-  outcome 

Instance Property

# outcome

The outcome of the transaction.

iOS 16.4+iPadOS 16.4+Mac Catalyst 17.0+

``` source
let outcome: PaymentCardReadResult.ReadOutcome
```

## Discussion

This field is meaningful only if you enable includeErrorInReadResult before you call prepare(using:). If an error occurs while the PaymentCardReaderSession is open and the framework can retrieve paymentCardData, PaymentCardReadResult includes both the PaymentCardReadResult.ReadOutcome and the other read data, otherwise the framework throws a PaymentCardReaderSession.ReadError.

## See Also

### Checking the read outcome

enum ReadOutcome

Values that describe the outcome of a read request.

