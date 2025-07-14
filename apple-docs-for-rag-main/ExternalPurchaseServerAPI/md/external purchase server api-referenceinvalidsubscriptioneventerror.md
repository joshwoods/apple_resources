

- External Purchase Server API
-  ReferenceInvalidSubscriptionEventError 

Object

# ReferenceInvalidSubscriptionEventError

External Purchase Server API 1.0.0+

``` source
object ReferenceInvalidSubscriptionEventError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `14`

`errorMessage`

`string`

 (Required) 

Value: `The referenced line item has no subscription event or its subscription event is not SUBSCRIPTION_START.`

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

