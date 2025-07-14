

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  PKPaymentRequest.MerchantCategoryCode 

Structure

# PKPaymentRequest.MerchantCategoryCode

An optional four-digit struct, in ISO 18245 format, that represents the type of goods or service the merchant provides for the transaction.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+visionOSwatchOS 11.0+

``` source
struct MerchantCategoryCode
```

## Overview

The four-digit merchant category codes are in ISO 18245 format and range from 1 to 9999.

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- LosslessStringConvertible
- RawRepresentable
- Sendable

## See Also

### Setting merchant information

var merchantIdentifier: String

Your merchant identifier.

var merchantCapabilities: PKMerchantCapability

A bit field of the payment-processing protocols and card types that you support.

struct PKMerchantCapability

Capabilities for processing payment.

