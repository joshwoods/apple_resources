

- External Purchase Server API
-  ReportingCurrencyExchangeNotAllowedError 

Object

# ReportingCurrencyExchangeNotAllowedError

External Purchase Server API 1.0.0+

``` source
object ReportingCurrencyExchangeNotAllowedError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `18`

`errorMessage`

`string`

 (Required) 

Value: `The reporting currency, which reports a currency exchange, isn't allowed.`

`fieldName`

`string`

 (Required) 

Value: `reportingCurrency`

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

