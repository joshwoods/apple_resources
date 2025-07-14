

- External Purchase Server API
-  SubscriptionStartNonZeroDaysPaidServiceError 

Object

# SubscriptionStartNonZeroDaysPaidServiceError

External Purchase Server API 1.0.0+

``` source
object SubscriptionStartNonZeroDaysPaidServiceError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `34`

`errorMessage`

`string`

 (Required) 

Value: `The subscriptionDaysOfPaidService field must be zero for a line item with subscription event SUBSCRIPTION_START.`

`fieldName`

`string`

 (Required) 

Value: `subscriptionDaysOfPaidService`

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

