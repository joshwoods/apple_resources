

- External Purchase Server API
-  UnknownEnumError 

Object

# UnknownEnumError

External Purchase Server API 1.0.0+

``` source
object UnknownEnumError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `7`

`errorMessage`

`string`

 (Required) 

Value: `The provided value is unknown for an enumeration.`

`fieldName`

`string`

 (Required) 

Possible Values: `reportingCurrency, taxCountry`

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

