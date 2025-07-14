

- External Purchase Server API
-  DuplicateValueError 

Object

# DuplicateValueError

External Purchase Server API 1.0.0+

``` source
object DuplicateValueError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `1`

`errorMessage`

`string`

 (Required) 

Value: `The field's value is already submitted and a duplicate value is not expected.`

`fieldName`

`string`

 (Required) 

Possible Values: `requestIdentifier, lineItemId`

`lineItemId`

lineItemId

## See Also

### Error objects for reports

object DateTooFarInPastError

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

object NetAmountMismatchError

