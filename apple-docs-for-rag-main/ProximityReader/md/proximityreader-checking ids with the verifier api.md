

- ProximityReader
-  Checking IDs with the Verifier API 

Sample Code

# Checking IDs with the Verifier API

Read and verify mobile driver’s license information without any additional hardware.

Download

iOS 17.0+Xcode 15.0+

## Overview

Note

This sample code project is associated with WWDC23 session 10114: What’s new in Wallet and Apple Pay.

### Configure the sample code project

The project contains two targets:

- `VerifierAPISample-DisplayRequest`: This target is configured to perform a MobileDriversLicenseDisplayRequest.

- `VerifierAPISample-DataRequest`: This target is configured to perform a MobileDriversLicenseDataRequest.

## See Also

### Mobile document reader

Adopting the Verifier API in your iPhone app

Configure and test ID Verifier support in your app for reading mobile documents.

Generating reader tokens for the Verifier API

Configure your server to generate reader tokens to prepare a device for mobile document reading.

class MobileDocumentReader

An object for configuring mobile document reading on the current device.

class MobileDocumentReaderSession

The object you use to start reading a mobile document.

