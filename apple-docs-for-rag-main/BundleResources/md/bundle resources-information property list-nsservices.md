

- Bundle Resources
- Information Property List
-  NSServices 

Property List Key

# NSServices

The services provided by an app.

macOS 10.0+

## Details 

Name  
Services

Type  

array of dictionaries

## Topics

### Invocation

NSKeyEquivalent

A keyboard shortcut that invokes the service menu command.

**Name:** Menu key equivalent

NSMenuItem

Text for a Services menu item.

**Name:** Menu

NSMessage

An instance method that invokes the service.

**Name:** Instance method name

NSPortName

The port that the service monitors for incoming requests.

**Name:** Incoming service port name

NSTimeout

The amount of time, in milliseconds, that the system waits for a response from the service.

**Name:** Timeout value (in milliseconds)

### Data

NSReturnTypes

The data types that the service returns.

**Name:** Return Types

NSSendTypes

The data types that the service can read.

**Name:** Send Types

NSUserData

A service-specific string value.

**Name:** User Data

## See Also

### Extensions and services

NSExtension

The properties of an app extension.

WKExtensionDelegateClassName

The name of your watchOS app’s extension delegate.

UIApplicationShortcutWidget

The bundle ID of the widget that’s available as a Home screen quick action in apps that have more than one widget.

**Name:** Home Screen Widget

