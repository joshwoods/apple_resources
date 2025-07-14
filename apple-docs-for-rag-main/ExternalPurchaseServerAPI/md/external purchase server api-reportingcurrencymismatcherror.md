

- External Purchase Server API
-  ReportingCurrencyMismatchError 

Object

# ReportingCurrencyMismatchError

External Purchase Server API 1.0.0+

``` source
object ReportingCurrencyMismatchError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `2`

`errorMessage`

`string`

 (Required) 

Value: `The refund's referenced buy line item has a different reporting currency.`

`fieldName`

`string`

 (Required) 

Value: `reportingCurrency`

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

