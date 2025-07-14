

- External Purchase Server API
-  PositiveValueRequiredError 

Object

# PositiveValueRequiredError

External Purchase Server API 1.0.0+

``` source
object PositiveValueRequiredError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `16`

`errorMessage`

`string`

 (Required) 

Value: `This field requires a positive value.`

`fieldName`

`string`

 (Required) 

Possible Values: `quantity, exchangeRate`

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

