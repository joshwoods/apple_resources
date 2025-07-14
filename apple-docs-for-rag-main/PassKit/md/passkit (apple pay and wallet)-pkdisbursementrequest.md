

- PassKit (Apple Pay and Wallet)
-  PKDisbursementRequest 

Class

# PKDisbursementRequest

An object that represents a request to disburse funds from a merchant to an individual.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
class PKDisbursementRequest
```

## Overview

Use this object to create a disbursement (payment) request from a merchant to a user account — for example, a withdrawal from an online account.

## Topics

### Initializers

convenience init(merchantIdentifier: String, currency: Locale.Currency, region: Locale.Region, supportedNetworks: [PKPaymentNetwork], merchantCapabilities: PKMerchantCapability, summaryItems: [PKPaymentSummaryItem])

Creates a disbursement request with the parameters you specify.

### Setting currency and region information

var currency: Locale.Currency

The currency to use for this disbursement.

var region: Locale.Region

The geographic region that describes the location for this disbursement.

var supportedRegions: [Locale.Region]?

An array of regions that describe the locations to support.

### Setting the summary items

var summaryItems: [PKPaymentSummaryItem]

An array of payment summary item objects that the framework presents to people.

class PKPaymentSummaryItem

An object that defines a summary item in a payment request, taxes, discounts, shipping, a grand total, and the like.

class PKDisbursementSummaryItem

A summary item that represents a disbursement.

class PKInstantFundsOutFeeSummaryItem

A summary item that represents a fee for an instant funds out transfer.

### Setting custom application data

var applicationData: Data?

Optional merchant-supplied information about the disbursement request.

### Setting the merchant information

var merchantIdentifier: String

A string that identifies the merchant.

var merchantCapabilities: PKMerchantCapability

A value that represents the payment-processing capabilities of the merchant.

var supportedNetworks: [PKPaymentNetwork]

An array of payment networks the merchant supports.

### Requesting recipient contact fields

var recipientContact: PKContact?

A contact object that describes the recipient.

var requiredRecipientContactFields: [PKContactField]

An array that indicates which of the recipient’s contact details the merchant requires in order to process a disbursement.

### Handling errors

class func disbursementCardUnsupportedError() -> any Error

Creates an error that indicates that the selected payment pass doesn’t support receiving funds through disbursements.

class func disbursementContactInvalidError(withContactField: PKContactField, localizedDescription: String?) -> any Error

Creates a recipient contact error with the supplied field.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

