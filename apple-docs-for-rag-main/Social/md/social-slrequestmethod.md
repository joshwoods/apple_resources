

- Social
-  SLRequestMethod 

Enumeration

# SLRequestMethod

Indicates the request method used in the request.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 10.8+

``` source
enum SLRequestMethod
```

## Overview

Use this constant to set the requestMethod property. The type of request to use depends on the target service. For links to documentation for the supported services, see Table 1 in SLRequest.

## Topics

### Constants

case GET

Requests information from the specified resource.

case POST

Submits data to be processed.

case DELETE

Deletes the specified resource.

case PUT

Uses a PUT request to submit the data.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Request Details

func preparedURLRequest() -> URLRequest!

Returns an authorized URL request that can be sent using an NSURLConnection object.

var requestMethod: SLRequestMethod

The method to use for this request.

var url: URL!

The destination URL for this request.

var parameters: [AnyHashable : Any]!

The parameters for this request.

