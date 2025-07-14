

- External Purchase Server API
-  ReferenceLineItemNotABuyError 

Object

# ReferenceLineItemNotABuyError

External Purchase Server API 1.0.0+

``` source
object ReferenceLineItemNotABuyError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `21`

`errorMessage`

`string`

 (Required) 

Value: `The referenced line item is not a buy.`

`fieldName`

`string`

 (Required) 

Value: `referenceLineItemId`

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

