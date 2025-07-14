

- External Purchase Server API
-  IncorrectAmountTaxInclusiveError 

Object

# IncorrectAmountTaxInclusiveError

External Purchase Server API 1.0.0+

``` source
object IncorrectAmountTaxInclusiveError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `11`

`errorMessage`

`string`

 (Required) 

Value: `The tax exclusive amount plus the tax amount does not equal the tax inclusive amount.`

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

object IncorrectNetAmountError

object InvalidTaxInclusiveAmountForSubscriptionPaymentError

object LineItemStatusRegressionError

object LineItemsNotAllowedForStatusError

object MaximumLengthExceededError

object MissingLineItemsForStatusError

object NegativeValueNotAllowedError

object NetAmountMismatchError

