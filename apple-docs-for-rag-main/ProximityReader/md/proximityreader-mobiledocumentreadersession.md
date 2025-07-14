

- ProximityReader
-  MobileDocumentReaderSession 

Class

# MobileDocumentReaderSession

The object you use to start reading a mobile document.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
final class MobileDocumentReaderSession
```

## Mentioned in 

Adopting the Verifier API in your iPhone app

Generating reader tokens for the Verifier API

## Overview

Use a `MobileDocumentReaderSession` object to read mobile documents from a properly configured device. Don’t create this object directly. Instead, obtain one by calling the prepare(using:) method of your MobileDocumentReader object. This returns a session after the successful configuration of the device.

Maintain a strong reference to a session object for the duration of the document-reading process. You may use the same session object to perform multiple read operations, but you may perform only one read operation at a time from the device.

## Topics

### Performing a document request

func requestDocument&lt;Request>(Request) async throws -> Request.Response

Presents a sheet to read a mobile document and returns the relevant response.

## Relationships

### Conforms To

- Sendable

## See Also

### Mobile document reader

Adopting the Verifier API in your iPhone app

Configure and test ID Verifier support in your app for reading mobile documents.

Generating reader tokens for the Verifier API

Configure your server to generate reader tokens to prepare a device for mobile document reading.

Checking IDs with the Verifier API

Read and verify mobile driver’s license information without any additional hardware.

class MobileDocumentReader

An object for configuring mobile document reading on the current device.

