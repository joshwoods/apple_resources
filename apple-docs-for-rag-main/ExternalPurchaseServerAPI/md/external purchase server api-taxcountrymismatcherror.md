

- External Purchase Server API
-  TaxCountryMismatchError 

Object

# TaxCountryMismatchError

External Purchase Server API 1.0.0+

``` source
object TaxCountryMismatchError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `23`

`errorMessage`

`string`

 (Required) 

Value: `The refund's referenced buy line item has a different tax country.`

`fieldName`

`string`

 (Required) 

Value: `taxCountry`

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

