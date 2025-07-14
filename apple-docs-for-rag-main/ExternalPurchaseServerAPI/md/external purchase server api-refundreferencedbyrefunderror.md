

- External Purchase Server API
-  RefundReferencedByRefundError 

Object

# RefundReferencedByRefundError

External Purchase Server API 1.0.0+

``` source
object RefundReferencedByRefundError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `28`

`errorMessage`

`string`

 (Required) 

Value: `The line item has event type REFUND but is referenced by a different line item that also has event type REFUND.`

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

