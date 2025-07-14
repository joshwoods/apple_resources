

- ProximityReader
- MobileNationalIDCardRawDataRequest
-  retainedElements 

Instance Property

# retainedElements

The document elements you’re requesting and intend to retain for an indefinite period of time.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
var retainedElements: [MobileNationalIDCardRawDataRequest.Element]
```

## See Also

### Configuring the request details

var region: Locale.Region

The region of the document you’re requesting.

var nonRetainedElements: [MobileNationalIDCardRawDataRequest.Element]

The document elements you’re requesting and intend to retain no longer than is necessary to process the result in realtime.

struct Element

A type representing an element that you can request from a mobile national ID card.

