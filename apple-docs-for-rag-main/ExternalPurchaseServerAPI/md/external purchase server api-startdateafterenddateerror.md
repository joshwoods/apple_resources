

- External Purchase Server API
-  StartDateAfterEndDateError 

Object

# StartDateAfterEndDateError

External Purchase Server API 1.0.0+

``` source
object StartDateAfterEndDateError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `17`

`errorMessage`

`string`

 (Required) 

Value: `The start date is after the end date.`

`fieldName`

`string`

 (Required) 

Value: `subscriptionEndDate`

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

