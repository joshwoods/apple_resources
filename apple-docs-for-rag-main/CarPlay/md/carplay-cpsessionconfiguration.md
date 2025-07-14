

- CarPlay
-  CPSessionConfiguration 

Class

# CPSessionConfiguration

An object that provides vehicle properties and configuration for the CarPlay environment.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPSessionConfiguration
```

## Overview

You use a session configuration to determine any user interface limits the vehicle imposes, such as keyboard display and list length, and the content style the vehicle selects according to the ambient light level.

## Topics

### Creating a Session Configuration

init(delegate: any CPSessionConfigurationDelegate)

Creates a session configuration with a delegate.

protocol CPSessionConfigurationDelegate

A protocol for receiving notifications about changes to vehicle properties and configuration.

### Managing the Delegate

var delegate: (any CPSessionConfigurationDelegate)?

An object that serves as the delegate to the session configuration.

### Getting the Content Style

var contentStyle: CPContentStyle

The content style that the vehicle selects.

struct CPContentStyle

The types of content style that the vehicle allows.

### Getting the Limits

var limitedUserInterfaces: CPLimitableUserInterface

A bit mask value that indicates the user interface limits.

struct CPLimitableUserInterface

The types of limitable user interface elements.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### CarPlay Integration

Requesting CarPlay Entitlements

Configure your CarPlay-enabled app with the entitlements it requires.

Displaying Content in CarPlay

Use scenes to present your app’s content on the vehicle’s built-in screen.

Supporting Previous Versions of iOS

Make your CarPlay-enabled apps compatible with older system versions, such as iOS 13 and earlier.

Using the CarPlay Simulator

Configure Simulator to run and debug your CarPlay-enabled app.

class CPTemplateApplicationScene

A CarPlay scene that controls your app’s user interface.

protocol CPTemplateApplicationSceneDelegate

The methods for responding to the life cycle events of your app’s scene.

