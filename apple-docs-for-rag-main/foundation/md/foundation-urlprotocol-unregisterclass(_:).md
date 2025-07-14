

- Foundation
- URLProtocol
-  unregisterClass(\_:) 

Type Method

# unregisterClass(\_:)

Unregisters the specified subclass of URLProtocol.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func unregisterClass(_ protocolClass: AnyClass)
```

## Parameters 

`protocolClass`  

The subclass of URLProtocol to unregister.

## Discussion

After this method is invoked, `protocolClass` is no longer consulted by the URL loading system.

## See Also

### Registering and unregistering protocol classes

class func registerClass(AnyClass) -> Bool

Attempts to register a subclass of URLProtocol, making it visible to the URL loading system.

