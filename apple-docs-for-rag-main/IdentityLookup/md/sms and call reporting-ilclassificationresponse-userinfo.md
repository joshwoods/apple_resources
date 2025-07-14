

- SMS and Call Reporting
- ILClassificationResponse
-  userInfo 

Instance Property

# userInfo

JSON data included in a response sent over the network.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
var userInfo: [String : Any]? { get set }
```

## Discussion

Use this property if you set the `ILClassificationExtensionNetworkReportDestination` key in the extension’s `Info.plist` file. The property stores any additional data that you want to pass to your servers as part of the response. Both the keys and values must be JSON-serializable. For more information, see NSJSONSerialization.

## See Also

### Accessing Data

var action: ILClassificationAction

A classification that determines what action the system takes.

var userString: String?

Text included in a response sent over SMS.

