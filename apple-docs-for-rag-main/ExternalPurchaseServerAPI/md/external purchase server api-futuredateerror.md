

- External Purchase Server API
-  FutureDateError 

Object

# FutureDateError

External Purchase Server API 1.0.0+

``` source
object FutureDateError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `6`

`errorMessage`

`string`

 (Required) 

Value: `The provided date field is in the future and future values are not allowed.`

`fieldName`

`string`

 (Required) 

Value: `creationDate`

`lineItemId`

lineItemId

## See Also

### Error objects for reports

object DateTooFarInPastError

object DuplicateValueError

object ErroneousLineItemReferencedByValidLineItemError

object ErroneouslySubmittedNotRestatementError

object ExchangeRateMismatchError

object FieldNotAllowedError

object IncorrectAmountTaxInclusiveError

object IncorrectNetAmountError

object InvalidTaxInclusiveAmountForSubscriptionPaymentError

object LineItemStatusRegressionError

object LineItemsNotAllowedForStatusError

object MaximumLengthExceededError

object MissingLineItemsForStatusError

object NegativeValueNotAllowedError

object NetAmountMismatchError

