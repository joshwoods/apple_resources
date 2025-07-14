

- Watch Connectivity
- WCSession
-  isSupported() 

Type Method

# isSupported()

Returns a Boolean value indicating whether the current iOS device is able to use a session object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func isSupported() -> Bool
```

## Return Value

true if a session object is available or false if it is not.

## Discussion

Before retrieving the default session object, call this method to verify that the current device supports watch connectivity. Session objects are always available on Apple Watch. They are also available on iPhones that support pairing with an Apple Watch. For all other devices, this method returns false to indicate that you cannot use the classes and methods of this framework.

## See Also

### Getting the Default Session

class var `default`: WCSession

Returns the singleton session object for the current device.

