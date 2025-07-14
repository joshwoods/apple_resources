

- Foundation
- NSXPCListener
-  anonymous() 

Type Method

# anonymous()

Returns a new anonymous listener connection.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func anonymous() -> NSXPCListener
```

## Discussion

Other processes can connect to this listener by passing this listener object’s `NSXPCListenerEndpoint` to the init(listenerEndpoint:) method of an NSXPCConnection object.

## See Also

### Using standard listeners

class func service() -> NSXPCListener

Returns the singleton listener used to listen for incoming connections in an XPC service.

