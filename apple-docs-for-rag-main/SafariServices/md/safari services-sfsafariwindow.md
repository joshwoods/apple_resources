

- Safari Services
-  SFSafariWindow 

Class

# SFSafariWindow

A proxy for a Safari window.

macOS 10.12+

``` source
class SFSafariWindow
```

## Mentioned in 

Adjusting settings for a toolbar item

## Topics

### Working with Tabs

func getActiveTab(completionHandler: (SFSafariTab?) -> Void)

Calls the completion handler with the active tab in the target window.

func openTab(with: URL, makeActiveIfPossible: Bool, completionHandler: ((SFSafariTab?) -> Void)?)

Opens a tab at the end of the tab bar.

### Getting the Toolbar Item

func getToolbarItem(completionHandler: (SFSafariToolbarItem?) -> Void)

Gets the extension’s toolbar item from the target window.

### Instance Methods

func close()

func getAllTabs(completionHandler: ([SFSafariTab]) -> Void)

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

class SFSafariPage

A proxy for a Safari webpage.

class SFSafariTab

A proxy for a tab in a Safari window.

