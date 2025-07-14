

- Foundation
- URLProtocol
-  registerClass(\_:) 

Type Method

# registerClass(\_:)

Attempts to register a subclass of URLProtocol, making it visible to the URL loading system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func registerClass(_ protocolClass: AnyClass) -> Bool
```

## Parameters 

`protocolClass`  

The subclass to register.

## Return Value

true if the registration is successful, false otherwise. The only failure condition is if `protocolClass` is not a subclass of URLProtocol.

## Discussion

Register any custom URLProtocol subclasses prior to making URL requests. When the URL loading system begins to load a request, it tries to initialize each registered protocol class with the specified request. The first URLProtocol subclass to return true when sent a canInit(with:) message is used to load the request. There is no guarantee that all registered protocol classes will be consulted.

Classes are consulted in the reverse order of their registration. A similar design governs the process to create the canonical form of a request with canonicalRequest(for:).

## See Also

### Registering and unregistering protocol classes

class func unregisterClass(AnyClass)

Unregisters the specified subclass of URLProtocol.

