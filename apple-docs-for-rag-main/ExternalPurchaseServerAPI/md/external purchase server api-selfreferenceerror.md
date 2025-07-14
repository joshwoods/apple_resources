

- External Purchase Server API
-  SelfReferenceError 

Object

# SelfReferenceError

External Purchase Server API 1.0.0+

``` source
object SelfReferenceError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `13`

`errorMessage`

`string`

 (Required) 

Value: `The line item may not reference itself.`

`fieldName`

`string`

 (Required) 

Value: `referenceLineItemId`

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

