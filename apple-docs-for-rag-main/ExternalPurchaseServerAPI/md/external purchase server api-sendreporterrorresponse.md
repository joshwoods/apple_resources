

- External Purchase Server API
-  SendReportErrorResponse 

Object

# SendReportErrorResponse

An error response that indicates your external purchase report didn’t succeed, including error details for the line items in your report.

External Purchase Server API 1.0.0+

``` source
object SendReportErrorResponse
```

## Properties

`errors`

`[*]`

 (Required) 

Possible types: DuplicateValueError`, `ReportingCurrencyMismatchError`, `NotFoundError`, `OmittedFieldError`, `FieldNotAllowedError`, `FutureDateError`, `UnknownEnumError`, `LineItemStatusRegressionError`, `MissingLineItemsForStatusError`, `LineItemsNotAllowedForStatusError`, `IncorrectAmountTaxInclusiveError`, `IncorrectNetAmountError`, `SelfReferenceError`, `ReferenceInvalidSubscriptionEventError`, `NegativeValueNotAllowedError`, `PositiveValueRequiredError`, `StartDateAfterEndDateError`, `ReportingCurrencyExchangeNotAllowedError`, `MaximumLengthExceededError`, `ErroneouslySubmittedNotRestatementError`, `ReferenceLineItemNotABuyError`, `ErroneousLineItemReferencedByValidLineItemError`, `TaxCountryMismatchError`, `NetAmountMismatchError`, `ValidLineItemReferencesErroneousLineItemError`, `SimultaneousSubmissionError`, `DateTooFarInPastError`, `RefundReferencedByRefundError`, `NonInitialBuyReferencedByBuyError`, `RepeatErroneousSubmissionError`, `ReferencedCreationDateIncompatibleError`, `PricingCurrencyMismatchError`, `ExchangeRateMismatchError`, `SubscriptionStartNonZeroDaysPaidServiceError`, `InvalidTaxInclusiveAmountForSubscriptionPaymentError

## See Also

### External purchase reporting

Send External Purchase Report

Report required information about external purchase tokens and associated transactions.

object ExternalPurchaseReport

The contents of an external purchase report for a single token.

object SendReportSuccessResponse

A response that contains the request identifier and indicates the server successfully received your external purchase report.

