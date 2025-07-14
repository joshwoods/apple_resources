

- External Purchase Server API
-  DateTooFarInPastError 

Object

# DateTooFarInPastError

External Purchase Server API 1.0.0+

``` source
object DateTooFarInPastError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `27`

`errorMessage`

`string`

 (Required) 

Value: `The provided date is too far in the past. Date must be in milliseconds.`

`fieldName`

`string`

 (Required) 

Possible Values: `creationDate, subscriptionStartDate, subscriptionEndDate`

`lineItemId`

lineItemId

## See Also

### Error objects for reports

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

object NetAmountMismatchError

