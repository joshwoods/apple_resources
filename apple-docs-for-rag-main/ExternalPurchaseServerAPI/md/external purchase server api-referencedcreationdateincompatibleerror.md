

- External Purchase Server API
-  ReferencedCreationDateIncompatibleError 

Object

# ReferencedCreationDateIncompatibleError

External Purchase Server API 1.0.0+

``` source
object ReferencedCreationDateIncompatibleError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `31`

`errorMessage`

`string`

 (Required) 

Value: `The referenced line item has a creation date after the line item's creation date.`

`fieldName`

`string`

 (Required) 

Value: `creationDate`

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

