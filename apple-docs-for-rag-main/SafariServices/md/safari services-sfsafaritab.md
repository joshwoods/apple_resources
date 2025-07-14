

- Safari Services
-  SFSafariTab 

Class

# SFSafariTab

A proxy for a tab in a Safari window.

macOS 10.12+

``` source
class SFSafariTab
```

## Topics

### Accessing Pages

func getActivePage(completionHandler: (SFSafariPage?) -> Void)

Calls the completion handler passing the active page in the tab.

func getPagesWithCompletionHandler(([SFSafariPage]?) -> Void)

Calls the completion handler with all of the tab’s active and preloading pages.

### Activating Tabs

func activate(completionHandler: (() -> Void)?)

Activates the tab.

### Instance Methods

func close()

func getContainingWindow(completionHandler: (SFSafariWindow?) -> Void)

func navigate(to: URL)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Safari app extensions

Safari app extensions

Learn how Safari app extensions extend the web-browsing experience in Safari by leveraging web technologies and native code.

class SFSafariExtension

A proxy for the Safari extension.

class SFSafariApplication

A proxy for the Safari app.

class SFSafariWindow

A proxy for a Safari window.

class SFSafariPage

A proxy for a Safari webpage.

