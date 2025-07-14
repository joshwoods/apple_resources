

- External Purchase Server API
-  Error messages and codes 

API Collection

# Error messages and codes

Error messages and codes for reports and endpoints.

## Topics

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

object NetAmountMismatchError

object NonInitialBuyReferencedByBuyError

object NotFoundError

object OmittedFieldError

object PositiveValueRequiredError

object PricingCurrencyMismatchError

object ReferenceInvalidSubscriptionEventError

object ReferenceLineItemNotABuyError

object ReferencedCreationDateIncompatibleError

object RefundReferencedByRefundError

object RepeatErroneousSubmissionError

object ReportingCurrencyExchangeNotAllowedError

object ReportingCurrencyMismatchError

object SelfReferenceError

object SimultaneousSubmissionError

object StartDateAfterEndDateError

object SubscriptionStartNonZeroDaysPaidServiceError

object TaxCountryMismatchError

object UnknownEnumError

object ValidLineItemReferencesErroneousLineItemError

### Error types

type errorCode

An integer value that represents an error in the External Purchase Server API.

type errorMessage

A string that describes an error.

type fieldName

A string that names a field of a line item.

