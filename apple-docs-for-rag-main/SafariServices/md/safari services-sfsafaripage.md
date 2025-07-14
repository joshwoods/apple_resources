

- Safari Services
-  SFSafariPage 

Class

# SFSafariPage

A proxy for a Safari webpage.

macOS 10.12+

``` source
class SFSafariPage
```

## Overview

Use an `SFSafariPage` object in your Safari app extension to send messages to injected content scripts, access page properties, and reload the page.

## Topics

### Messaging Injected Scripts

func dispatchMessageToScript(withName: String, userInfo: [String : Any]?)

Dispatches a message from the app extension to the content script injected in this page.

### Getting Page Information

func getPropertiesWithCompletionHandler((SFSafariPageProperties?) -> Void)

Retrieves the properties of the webpage.

### Reloading the Page

func reload()

Tells Safari to reload the webpage.

### Instance Methods

func getContainingTab(completionHandler: (SFSafariTab) -> Void)

func getScreenshotOfVisibleArea(completionHandler: (NSImage?) -> Void)

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

class SFSafariTab

A proxy for a tab in a Safari window.

