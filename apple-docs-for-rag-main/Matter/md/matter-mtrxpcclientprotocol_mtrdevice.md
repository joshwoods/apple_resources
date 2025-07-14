

- Matter
-  MTRXPCClientProtocol_MTRDevice 

Protocol

# MTRXPCClientProtocol_MTRDevice

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
protocol MTRXPCClientProtocol_MTRDevice : NSObjectProtocol
```

## Topics

### Instance Methods

func device(NSNumber, internalStateUpdated: [AnyHashable : Any])

**Required**

func device(NSNumber, receivedAttributeReport: [[String : Any]])

**Required**

func device(NSNumber, receivedEventReport: [[String : Any]])

**Required**

func device(NSNumber, stateChanged: MTRDeviceState)

**Required**

func deviceBecameActive(NSNumber)

**Required**

func deviceCachePrimed(NSNumber)

**Required**

func deviceConfigurationChanged(NSNumber)

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- MTRXPCClientProtocol

