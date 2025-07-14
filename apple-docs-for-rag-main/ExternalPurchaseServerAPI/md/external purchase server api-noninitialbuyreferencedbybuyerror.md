

- External Purchase Server API
-  NonInitialBuyReferencedByBuyError 

Object

# NonInitialBuyReferencedByBuyError

External Purchase Server API 1.0.0+

``` source
object NonInitialBuyReferencedByBuyError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `29`

`errorMessage`

`string`

 (Required) 

Value: `The line item does not have subscription event INITIAL_BUY but it is referenced by a subscription line item with event type BUY.`

`fieldName`

`string`

 (Required) 

Value: `lineItemId`

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

