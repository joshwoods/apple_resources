

- Safari Services
-  SFSafariExtensionHandler 

Class

# SFSafariExtensionHandler

A base class that you subclass to handle events in your Safari app extension.

macOS 10.12+

``` source
class SFSafariExtensionHandler
```

## Mentioned in 

Adjusting settings for contextual menu items

Building a Safari app extension

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSExtensionRequestHandling
- NSObjectProtocol
- SFSafariExtensionHandling

## See Also

### Injected style sheets and scripts

Using injected style sheets and scripts

Learn how you can affect the appearance or behavior of a webpage by using injected style sheets and scripts.

Injecting a script into a webpage

Inject a script that you write for a Safari app extension into a webpage.

Injecting CSS style sheets into a webpage

Add to or override styles by injecting CSS style sheets into webpages.

Passing messages between Safari app extensions and injected scripts

Communicate between your Safari app extension and injected scripts.

class SFSafariExtensionManager

A class that your app uses to find out the current state of a Safari app extension.

class SFSafariExtensionState

The state of a Safari app extension.

class SFSafariPageProperties

An object that captures information about a webpage.

protocol SFSafariExtensionHandling

A protocol for implementing event handling in a Safari app extension.

let SFExtensionProfileKey: String

A string the system uses as a key in a user info dictionary to identify a profile identifier.

