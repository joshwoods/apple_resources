

- Foundation
- NSXPCListener
-  endpoint 

Instance Property

# endpoint

Returns an endpoint object that may be sent over an existing connection.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var endpoint: NSXPCListenerEndpoint { get }
```

## Discussion

The receiver of the endpoint can use this object to create a new connection to this NSXPCListener object. The resulting `NSXPCListenerEndpoint` object uniquely names this listener object across connections.

## See Also

### Related Documentation

Daemons and Services Programming Guide

