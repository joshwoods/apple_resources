

- WebKit
-  WebArchive Deprecated

Class

# WebArchive

A WebArchive object represents a webpage that can be archived—for example, archived on disk or on the pasteboard. A WebArchive object contains the main resource, as well as the subresources and subframes of the main resource. The main resource can be an entire webpage, a portion of a webpage, or some other kind of data such as an image. Use this class to archive webpages, or place a portion of a webpage on the pasteboard, or to represent rich web content in any application.

macOS 10.3–10.14Deprecated

``` source
class WebArchive
```

## Topics

### Initializing

init!(mainResource: WebResource!, subresources: [Any]!, subframeArchives: [Any]!)

Initializes the receiver with a resource and optional subresources and subframe archives..

init!(data: Data!)

Initializes and returns the receiver, specifying the initial content data.

### Getting attributes

var mainResource: WebResource!

The receiver’s main resource.

var subresources: [Any]!

The receiver’s subresources, or `nil` if there are none.

var subframeArchives: [Any]!

Archives representing the receiver’s subresources or `nil` if there are none.

var data: Data!

The data representation of the receiver.

### Constants

let WebArchivePboardType: String

The pasteboard type constant used when adding or accessing a WebArchive on the pasteboard.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

