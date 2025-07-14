

- External Purchase Server API
-  MaximumLengthExceededError 

Object

# MaximumLengthExceededError

External Purchase Server API 1.0.0+

``` source
object MaximumLengthExceededError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `19`

`errorMessage`

`string`

 (Required) 

Value: `The field's maximum length is exceeded.`

`fieldName`

`string`

 (Required) 

Possible Values: `referenceLineItemId, lineItemId, productIdentifier, pricingCurrency, exchangeRate`

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

object MissingLineItemsForStatusError

object NegativeValueNotAllowedError

object NetAmountMismatchError

