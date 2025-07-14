

- SMS and Call Reporting
-  ILNetworkResponse 

Class

# ILNetworkResponse

A response to an HTTPS network request performed on behalf of a Message Filter app extension.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
class ILNetworkResponse
```

## Overview

To preserve user privacy, a Message Filter app extension can’t contact the server itself. Instead, it tells the system to contact the server and pass back the server’s response.

## Topics

### Getting the Response

var urlResponse: HTTPURLResponse

Encapsulation of an HTTPS URL response.

### Getting Data from the Response

var data: Data

The data returned in the HTTPS response.

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
- NSObjectProtocol
- NSSecureCoding

## See Also

### Responses

class ILMessageFilterQueryResponse

A response to a message filter query request.

enum ILMessageFilterAction

Responds to a received message with a filter action.

