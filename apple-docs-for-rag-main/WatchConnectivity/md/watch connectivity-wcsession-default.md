

- Watch Connectivity
- WCSession
-  default 

Type Property

# default

Returns the singleton session object for the current device.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var `default`: WCSession { get }
```

## Return Value

The session object for the current device.

## Discussion

Call the isSupported() method before calling this method to make sure you can use session objects for communication.

## See Also

### Getting the Default Session

class func isSupported() -> Bool

Returns a Boolean value indicating whether the current iOS device is able to use a session object.

