

- ProximityReader
- MobileNationalIDCardDataRequest
-  region 

Instance Property

# region

The region of the document you’re requesting.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
var region: Locale.Region
```

## See Also

### Configuring the request details

var retainedElements: [MobileNationalIDCardDataRequest.Element]

The document elements you’re requesting and intend to retain for an indefinite period of time.

var nonRetainedElements: [MobileNationalIDCardDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than necessary to process the result in realtime.

struct Element

A type that represents an element you can request from a mobile national ID card.

