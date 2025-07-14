

- External Purchase Server API
-  RepeatErroneousSubmissionError 

Object

# RepeatErroneousSubmissionError

External Purchase Server API 1.0.0+

``` source
object RepeatErroneousSubmissionError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `30`

`errorMessage`

`string`

 (Required) 

Value: `The line item has status erroneously submitted but its previous version was already marked erroneously submitted.`

`fieldName`

`string`

 (Required) 

Value: `erroneouslySubmitted`

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

