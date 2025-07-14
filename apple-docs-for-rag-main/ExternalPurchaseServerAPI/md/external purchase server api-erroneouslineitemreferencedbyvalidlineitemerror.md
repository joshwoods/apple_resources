

- External Purchase Server API
-  ErroneousLineItemReferencedByValidLineItemError 

Object

# ErroneousLineItemReferencedByValidLineItemError

External Purchase Server API 1.0.0+

``` source
object ErroneousLineItemReferencedByValidLineItemError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `22`

`errorMessage`

`string`

 (Required) 

Value: `The line item has status erroneously submitted but is referenced by a non-erroneously submitted line item.`

`fieldName`

`string`

 (Required) 

Value: `erroneouslySubmitted`

`lineItemId`

lineItemId

 (Required) 

## See Also

### Error objects for reports

object DateTooFarInPastError

object DuplicateValueError

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

object NetAmountMismatchError

