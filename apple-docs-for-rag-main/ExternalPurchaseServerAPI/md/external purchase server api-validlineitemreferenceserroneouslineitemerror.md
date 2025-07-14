

- External Purchase Server API
-  ValidLineItemReferencesErroneousLineItemError 

Object

# ValidLineItemReferencesErroneousLineItemError

External Purchase Server API 1.0.0+

``` source
object ValidLineItemReferencesErroneousLineItemError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `25`

`errorMessage`

`string`

 (Required) 

Value: `The line item references an erroneously submitted line item, but the line item itself is not erroneously submitted.`

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

