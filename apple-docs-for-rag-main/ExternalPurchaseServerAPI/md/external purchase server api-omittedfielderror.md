

- External Purchase Server API
-  OmittedFieldError 

Object

# OmittedFieldError

External Purchase Server API 1.0.0+

``` source
object OmittedFieldError
```

## Properties

`errorCode`

`integer`

 (Required) 

Value: `4`

`errorMessage`

`string`

 (Required) 

Value: `A required field is missing.`

`fieldName`

`string`

 (Required) 

Possible Values: `requestIdentifier, externalPurchaseId, status, lineItemId, creationDate, eventType, referenceLineItemId, productIdentifier, productType, subscriptionEvent, subscriptionStartDate, subscriptionEndDate, subscriptionDaysOfPaidService, quantity, amountTaxExclusive, amountTaxInclusive, taxAmount, netAmountTaxExclusive, reportingCurrency, exchangeRate, pricingCurrency, taxCountry`

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

