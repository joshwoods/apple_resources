

- External Purchase Server API
-  InvalidTaxInclusiveAmountForSubscriptionPaymentError 

Object

# InvalidTaxInclusiveAmountForSubscriptionPaymentError

External Purchase Server API 1.0.0+

``` source
object InvalidTaxInclusiveAmountForSubscriptionPaymentError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `35`

`errorMessage`

`string`

 (Required) 

Value: `The tax inclusive amount must be positive for line items with subscription event SUBSCRIPTION_PAYMENT.`

`fieldName`

`string`

 (Required) 

Value: `amountTaxInclusive`

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

object LineItemStatusRegressionError

object LineItemsNotAllowedForStatusError

object MaximumLengthExceededError

object MissingLineItemsForStatusError

object NegativeValueNotAllowedError

object NetAmountMismatchError

