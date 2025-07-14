

- Foundation
- NSMutableURLRequest
-  networkServiceType 

Instance Property

# networkServiceType

The network service type of the connection.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var networkServiceType: NSURLRequest.NetworkServiceType { get set }
```

## Discussion

The network service type provides a hint to the operating system about what the underlying traffic is used for. This hint enhances the system’s ability to prioritize traffic, determine how quickly it needs to wake up the cellular or Wi-Fi radio, and so on. By providing accurate information, you improve the ability of the system to optimally balance battery life, performance, and other considerations.

For example, specify the NSURLRequest.NetworkServiceType.background type if your app is performing a download that was not requested by the user, like prefetching content so that it’s available when the user chooses to view it. By contrast, continually connected voice and video apps should use the NSURLRequest.NetworkServiceType.voice, NSURLRequest.NetworkServiceType.voip, or NSURLRequest.NetworkServiceType.video service types, as appropriate.

## See Also

### Accessing the service type

enum NetworkServiceType

Constants that specify how a request uses network resources.

