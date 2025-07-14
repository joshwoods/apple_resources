

- CarPlay
-  CPSessionConfigurationDelegate 

Protocol

# CPSessionConfigurationDelegate

A protocol for receiving notifications about changes to vehicle properties and configuration.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
protocol CPSessionConfigurationDelegate : NSObjectProtocol
```

## Topics

### Handling Content Style Changes

func sessionConfiguration(CPSessionConfiguration, contentStyleChanged: CPContentStyle)

Tells the delegate that the vehicle changed its selected content style.

### Handling Limit Changes

func sessionConfiguration(CPSessionConfiguration, limitedUserInterfacesChanged: CPLimitableUserInterface)

Tells the delegate that the system changed keyboard or list limits on the user interface.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Creating a Session Configuration

init(delegate: any CPSessionConfigurationDelegate)

Creates a session configuration with a delegate.

