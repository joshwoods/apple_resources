

- External Purchase Server API
-  LineItemsNotAllowedForStatusError 

Object

# LineItemsNotAllowedForStatusError

External Purchase Server API 1.0.0+

``` source
object LineItemsNotAllowedForStatusError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `10`

`errorMessage`

`string`

 (Required) 

Value: `A line item was provided for an external purchase ID that has a NO_LINE_ITEM or UNRECOGNIZED_TOKEN status.`

`fieldName`

`string`

 (Required) 

Value: `status`

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

object MaximumLengthExceededError

object MissingLineItemsForStatusError

object NegativeValueNotAllowedError

object NetAmountMismatchError

