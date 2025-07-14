

- SMS and Call Reporting
- ILClassificationResponse
-  userString 

Instance Property

# userString

Text included in a response sent over SMS.

iOS 12.1+iPadOS 12.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
var userString: String? { get set }
```

## Discussion

Use this property if you set the `ILClassificationExtensionSMSReportDestination` key in the extension’s `Info.plist` file. The string can store additional data that you want to pass in the SMS message.

## See Also

### Accessing Data

var action: ILClassificationAction

A classification that determines what action the system takes.

var userInfo: [String : Any]?

JSON data included in a response sent over the network.

