

- WebKit
-  WebResource 

Class

# WebResource

A `WebResource` object represents a downloaded URL. It encapsulates the data of the download as well as other resource properties such as the URL, MIME type, and frame name.

macOS

``` source
class WebResource
```

## Overview

Use the init(data:url:mimeType:textEncodingName:frameName:) method to initialize a newly created `WebResource` object. Use the other methods in this class to get the properties of a `WebResource` object.

## Topics

### Initializing

init!(data: Data!, url: URL!, mimeType: String!, textEncodingName: String!, frameName: String!)

Initializes and returns a web resource instance.

### Getting attributes

var data: Data!

The receiver’s data.

var url: URL!

The receiver’s URL.

var mimeType: String!

The receiver’s MIME type.

var textEncodingName: String!

The receiver’s text encoding name.

var frameName: String!

The name of the frame. If the receiver does not represent the contents of an entire HTML frame, this is `nil`.

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

### Loading Resources (Legacy)

protocol WebResourceLoadDelegate

Web view resource load delegates implement this protocol to be notified on the progress of loading individual resources. Note that there can be hundreds of resources, such as images and other media, per page. So, if you just want to get page loading status see the WebFrameLoadDelegate protocol.

Deprecated

