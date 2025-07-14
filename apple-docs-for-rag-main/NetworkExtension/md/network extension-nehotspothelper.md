

- Network Extension
-  NEHotspotHelper 

Class

# NEHotspotHelper

A class to register a hotspot helper.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class NEHotspotHelper
```

## Overview

The NEHotspotHelper API gives your app the ability to perform custom authentication for Wi-Fi Hotspots. It gives users a way to seamlessly connect to a large aggregated network of Wi-Fi Hotspots. The NEHotspotConfiguration API lets your app configure those hotspots.

## Topics

### Registering a hotspot helper

class func register(options: [String : NSObject]?, queue: dispatch_queue_t, handler: NEHotspotHelperHandler) -> Bool

Register the application as a Hotspot Helper.

let kNEHotspotHelperOptionDisplayName: String

The string displayed in Wi-Fi Settings for a network handled by the application.

typealias NEHotspotHelperHandler

The type definition for the Hotspot Helper’s command handler block.

### Getting hotspot network status

class func supportedNetworkInterfaces() -> [Any]?

Return the list of network interfaces managed by the Hotspot Helper infrastructure.

### Logging off

class func logoff(NEHotspotNetwork) -> Bool

Terminate the authentication session for a Hotspot network.

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

