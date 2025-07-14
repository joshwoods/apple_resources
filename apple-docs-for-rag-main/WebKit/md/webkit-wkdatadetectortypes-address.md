

- WebKit
- WKDataDetectorTypes
-  address 

Type Property

# address

Detect addresses in text and turn them into links to display the location.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
static var address: WKDataDetectorTypes { get }
```

## See Also

### Data Detector Types

static var phoneNumber: WKDataDetectorTypes

Detect phone numbers in text and create a link to call the specified number.

static var link: WKDataDetectorTypes

Detect URLs in text and turn them into links.

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

