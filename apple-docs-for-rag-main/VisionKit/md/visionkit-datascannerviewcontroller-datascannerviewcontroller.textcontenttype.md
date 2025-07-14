

- VisionKit
- DataScannerViewController
-  DataScannerViewController.TextContentType 

Enumeration

# DataScannerViewController.TextContentType

Types of text that a data scanner recognizes.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
enum TextContentType
```

## Mentioned in 

Scanning data with the camera

## Overview

To configure a DataScannerViewController, pass one or more options into its initializer. For example, the following code creates a data scanner that detects textual references to money.

```
```

## Topics

### Identifying content types

case URL

The content type for a URL that appears in text.

case dateTimeDuration

The content type for dates, times, and durations that appear in text.

case emailAddress

The content type for an email address that appears in text.

case flightNumber

The content type for a vendor-specific flight number that appears in text.

case fullStreetAddress

The content type for a mailing address that appears in text.

case shipmentTrackingNumber

The content type for a vendor-specific parcel tracking number that appears in text.

case telephoneNumber

The content type for a phone number that appears in text.

case currency

The content type for currency.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Recognizing text

static func text(languages: [String], textContentType: DataScannerViewController.TextContentType?) -> DataScannerViewController.RecognizedDataType

Creates a data type for text and information the scanner finds in text.

