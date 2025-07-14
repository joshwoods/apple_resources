

- External Purchase Server API
-  FieldNotAllowedError 

Object

# FieldNotAllowedError

External Purchase Server API 1.0.0+

``` source
object FieldNotAllowedError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `5`

`errorMessage`

`string`

 (Required) 

Value: `The provided field is not allowed.`

`fieldName`

`string`

 (Required) 

Possible Values: `productType, productIdentifier, subscriptionEvent, subscriptionStartDate, subscriptionEndDate, subscriptionDaysOfPaidService, quantity, referenceLineItemId, exchangeRate`

`lineItemId`

lineItemId

## See Also

### Error objects for reports

object DateTooFarInPastError

object DuplicateValueError

object ErroneousLineItemReferencedByValidLineItemError

object ErroneouslySubmittedNotRestatementError

object ExchangeRateMismatchError

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

