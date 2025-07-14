

- SMS and Call Reporting
-  ILClassificationResponse 

Class

# ILClassificationResponse

A response object that tells the system how to handle the reported communications.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
class ILClassificationResponse
```

## Overview

To work in areas where Wi-Fi connections and cellular data may be unreliable, the extension sends the response using an SMS message. As long as the action isn’t ILClassificationAction.none, the extension creates an SMS message to the number provided by the `ILClassificationExtensionSMSReportDestination` key in the extension’s `info.plist` file.

The message’s body contains a JSON string with both the classification action and the contents of the user info dictionary. For more information, see NSJSONSerialization.

## Topics

### Creating Responses

init(action: ILClassificationAction)

Creates a new response using the provided classification.

### Accessing Data

var action: ILClassificationAction

A classification that determines what action the system takes.

var userInfo: [String : Any]?

JSON data included in a response sent over the network.

var userString: String?

Text included in a response sent over SMS.

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

enum ILClassificationAction

The actions the system can take in response to the reported communication.

