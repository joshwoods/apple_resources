

- External Purchase Server API
-  ExchangeRateMismatchError 

Object

# ExchangeRateMismatchError

External Purchase Server API 1.0.0+

``` source
object ExchangeRateMismatchError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `33`

`errorMessage`

`string`

 (Required) 

Value: `The refund's referenced buy line item has a different exchange rate.`

`fieldName`

`string`

 (Required) 

Value: `exchangeRate`

`lineItemId`

lineItemId

 (Required) 

## See Also

### Error objects for reports

object DateTooFarInPastError

object DuplicateValueError

object ErroneousLineItemReferencedByValidLineItemError

object ErroneouslySubmittedNotRestatementError

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

