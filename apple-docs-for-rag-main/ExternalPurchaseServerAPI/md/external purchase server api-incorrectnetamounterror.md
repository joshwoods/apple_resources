

- External Purchase Server API
-  IncorrectNetAmountError 

Object

# IncorrectNetAmountError

External Purchase Server API 1.0.0+

``` source
object IncorrectNetAmountError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `12`

`errorMessage`

`string`

 (Required) 

Value: `The net amount value does not match the expected value.`

`fieldName`

`string`

 (Required) 

Value: `netAmountTaxExclusive`

`lineItemId`

lineItemId

 (Required) 

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

object InvalidTaxInclusiveAmountForSubscriptionPaymentError

object LineItemStatusRegressionError

object LineItemsNotAllowedForStatusError

object MaximumLengthExceededError

object MissingLineItemsForStatusError

object NegativeValueNotAllowedError

object NetAmountMismatchError

