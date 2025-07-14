

- AppKit
- NSWorkspace
-  NSWorkspace.OpenConfiguration 

Class

# NSWorkspace.OpenConfiguration

The configuration options for opening URLs or launching apps.

macOS 10.15+

``` source
class OpenConfiguration
```

## Overview

Create an NSWorkspace.OpenConfiguration object before launching an app or opening a URL using the shared NSWorkspace object. Use the properties of this object to customize the behavior of the launched app or the handling of the URLs. For example, you might tell the app to hide itself immediately after launch.

## Topics

### Handling URLs

var requiresUniversalLinks: Bool

A Boolean value indicating whether you require the URL to have an associated universal link.

var isForPrinting: Bool

A Boolean value indicating whether you want to print the contents of documents and URLs instead of opening them.

var requiresUniversalLinks: Bool

A Boolean value indicating whether you require the URL to have an associated universal link.

var isForPrinting: Bool

A Boolean value indicating whether you want to print the contents of documents and URLs instead of opening them.

### Specifying App-Related Behaviors

var activates: Bool

A Boolean value indicating whether the system activates the app and brings it to the foreground.

var addsToRecentItems: Bool

A Boolean value indicating whether to add the app or documents to the Recent Items menu.

var allowsRunningApplicationSubstitution: Bool

A Boolean value that indicates whether to use a running instance of an application even if it’s at a different URL.

var createsNewApplicationInstance: Bool

A Boolean value indicating whether you want the system to launch a new instance of the app.

var hides: Bool

A Boolean value indicating whether you want the app to hide itself after it launches.

var hidesOthers: Bool

A Boolean value indicating whether you want to hide all apps except the one that launched.

### Prompting the User

var promptsUserIfNeeded: Bool

A Boolean value indicating whether to display errors, authentication requests, or other UI elements to the user.

var promptsUserIfNeeded: Bool

A Boolean value indicating whether to display errors, authentication requests, or other UI elements to the user.

### Specifying Launch Attributes

var appleEvent: NSAppleEventDescriptor?

The first Apple event to send to the new app.

var arguments: [String]

The set of command-line arguments to pass to a new app instance at launch time.

var environment: [String : String]

The set of environment variables to set in a new app instance.

var architecture: cpu_type_t

The architecture version of the app to launch.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Environment

class NSWorkspace

A workspace that can launch other apps and perform a variety of file-handling services.

struct NSAppKitVersion

Constants for determining which version of AppKit is available.

LSMinimumSystemVersion

The minimum version of the operating system required for the app to run in macOS.

