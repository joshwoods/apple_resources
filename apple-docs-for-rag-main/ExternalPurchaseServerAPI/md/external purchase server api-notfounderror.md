

- External Purchase Server API
-  NotFoundError 

Object

# NotFoundError

External Purchase Server API 1.0.0+

``` source
object NotFoundError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `3`

`errorMessage`

`string`

 (Required) 

Value: `The referenced value was not found.`

`fieldName`

`string`

 (Required) 

Possible Values: `externalPurchaseId, lineItemId, referenceLineItemId, requestIdentifier`

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

