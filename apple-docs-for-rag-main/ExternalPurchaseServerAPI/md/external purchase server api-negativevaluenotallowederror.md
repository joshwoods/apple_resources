

- External Purchase Server API
-  NegativeValueNotAllowedError 

Object

# NegativeValueNotAllowedError

External Purchase Server API 1.0.0+

``` source
object NegativeValueNotAllowedError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `15`

`errorMessage`

`string`

 (Required) 

Value: `This field doesn't allow a negative value.`

`fieldName`

`string`

 (Required) 

Possible Values: `subscriptionDaysOfPaidService, netAmountTaxExclusive, taxAmount, amountTaxExclusive, amountTaxInclusive`

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

object NetAmountMismatchError

