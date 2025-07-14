

- External Purchase Server API
-  NetAmountMismatchError 

Object

# NetAmountMismatchError

External Purchase Server API 1.0.0+

``` source
object NetAmountMismatchError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `24`

`errorMessage`

`string`

 (Required) 

Value: `Two line items involved in the same net amount calculation have different net amount values.`

`fieldName`

`string`

 (Required) 

Value: `netAmountTaxExclusive`

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

object FutureDateError

object IncorrectAmountTaxInclusiveError

object IncorrectNetAmountError

object InvalidTaxInclusiveAmountForSubscriptionPaymentError

object LineItemStatusRegressionError

object LineItemsNotAllowedForStatusError

object MaximumLengthExceededError

object MissingLineItemsForStatusError

object NegativeValueNotAllowedError

