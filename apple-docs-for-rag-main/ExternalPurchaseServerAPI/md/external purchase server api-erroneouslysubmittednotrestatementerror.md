

- External Purchase Server API
-  ErroneouslySubmittedNotRestatementError 

Object

# ErroneouslySubmittedNotRestatementError

External Purchase Server API 1.0.0+

``` source
object ErroneouslySubmittedNotRestatementError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `20`

`errorMessage`

`string`

 (Required) 

Value: `Expecting restatement for an erroneously submitted line item, but line item is not a restatement.`

`fieldName`

`string`

 (Required) 

Value: `erroneouslySubmitted`

`lineItemId`

lineItemId

## See Also

### Error objects for reports

object DateTooFarInPastError

object DuplicateValueError

object ErroneousLineItemReferencedByValidLineItemError

object ExchangeRateMismatchError

object FieldNotAllowedError

object FutureDateError

object IncorrectAmountTaxInclusiveError

object IncorrectNetAmountError

object InvalidTaxInclusiveAmountForSubscriptionPaymentError

object LineItemStatusRegressionError

object LineItemsNotAllowedForStatusError

object MaximumLengthExceededError

object MissingLineItemsForStatusError

object NegativeValueNotAllowedError

object NetAmountMismatchError

