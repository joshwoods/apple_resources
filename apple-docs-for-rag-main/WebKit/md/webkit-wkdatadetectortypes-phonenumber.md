

- WebKit
- WKDataDetectorTypes
-  phoneNumber 

Type Property

# phoneNumber

Detect phone numbers in text and create a link to call the specified number.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
static var phoneNumber: WKDataDetectorTypes { get }
```

## See Also

### Data Detector Types

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

