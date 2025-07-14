

- External Purchase Server API
-  LineItemStatusRegressionError 

Object

# LineItemStatusRegressionError

External Purchase Server API 1.0.0+

``` source
object LineItemStatusRegressionError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `8`

`errorMessage`

`string`

 (Required) 

Value: `Cannot mark status as NO_LINE_ITEM or UNRECOGNIZED_TOKEN after previously reporting as LINE_ITEM.`

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

object LineItemsNotAllowedForStatusError

object MaximumLengthExceededError

object MissingLineItemsForStatusError

object NegativeValueNotAllowedError

object NetAmountMismatchError

