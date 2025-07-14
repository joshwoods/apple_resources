

- External Purchase Server API
-  PricingCurrencyMismatchError 

Object

# PricingCurrencyMismatchError

External Purchase Server API 1.0.0+

``` source
object PricingCurrencyMismatchError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `32`

`errorMessage`

`string`

 (Required) 

Value: `The refund's referenced buy line item has a different pricing currency.`

`fieldName`

`string`

 (Required) 

Value: `pricingCurrency`

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

