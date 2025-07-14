

- PassKit (Apple Pay and Wallet)
-  PKPaymentInformationRequestHandling 

Protocol

# PKPaymentInformationRequestHandling

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
protocol PKPaymentInformationRequestHandling
```

## Overview

Important

Before you can add a QR code purchase extension you need an entitlement from Apple. For more information on requesting an entitlement, contact apple-pay-inquiries@apple.com.

## Topics

### Getting the transaction information

func handle(PKBarcodeEventConfigurationRequest, completion: () -> Void)

**Required**

func handleInformationRequest(PKBarcodeEventMetadataRequest, completion: PKInformationRequestCompletionBlock)

**Required**

class PKBarcodeEventConfigurationRequest

class PKBarcodeEventMetadataRequest

class PKBarcodeEventMetadataResponse

typealias PKInformationRequestCompletionBlock

### Signing the transaction

func handle(PKBarcodeEventSignatureRequest, completion: PKSignatureRequestCompletionBlock)

**Required**

class PKBarcodeEventSignatureRequest

class PKBarcodeEventSignatureResponse

typealias PKSignatureRequestCompletionBlock

## See Also

### QR transaction information

class PKPaymentInformationEventExtension

An abstract superclass for an extension to collect payment information and sign transaction data in a QR code purchase.

