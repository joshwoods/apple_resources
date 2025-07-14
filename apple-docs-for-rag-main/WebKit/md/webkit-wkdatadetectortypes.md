

- WebKit
-  WKDataDetectorTypes 

Structure

# WKDataDetectorTypes

The data detector types.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct WKDataDetectorTypes
```

## Overview

To perform no data detection, create an empty set of data detector types, indicated by the empty array literal, `[]`. For example:

```
let myDataDetector: WKDataDetectorTypes = []
```

## Topics

### Data Detector Types

static var phoneNumber: WKDataDetectorTypes

Detect phone numbers in text and create a link to call the specified number.

static var link: WKDataDetectorTypes

Detect URLs in text and turn them into links.

static var address: WKDataDetectorTypes

Detect addresses in text and turn them into links to display the location.

static var calendarEvent: WKDataDetectorTypes

Turn future dates and times into links to create calendar events.

static var trackingNumber: WKDataDetectorTypes

Detect tracking numbers in text and turn them into links.

static var flightNumber: WKDataDetectorTypes

Detect flight numbers in text and turn them into links.

static var lookupSuggestion: WKDataDetectorTypes

Detect Spotlight suggestions and turn them into links.

static var all: WKDataDetectorTypes

Detect all data types and turn them into links.

### Initializers

init(rawValue: UInt)

### Deprecated Types

static var spotlightSuggestion: WKDataDetectorTypes

Spotlight suggestions are detected and turned into links.

Deprecated

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Identifying data types

var dataDetectorTypes: WKDataDetectorTypes

The types of data detectors to apply to the web view’s content.

