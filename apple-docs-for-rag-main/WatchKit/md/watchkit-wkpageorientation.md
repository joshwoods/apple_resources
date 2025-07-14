

- WatchKit
-  WKPageOrientation 

Enumeration

# WKPageOrientation

Scrolling orientations for page-based interfaces.

watchOS 4.0+

``` source
enum WKPageOrientation
```

## Topics

### Enumeration Cases

case horizontal

A horizontal page-based scrolling orientation.

case vertical

A vertical page-based scrolling orientation.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Navigating a page-based interface

class func reloadRootPageControllers(withNames: [String], contexts: [Any]?, orientation: WKPageOrientation, pageIndex: Int)

Loads the specified interface controllers and rebuilds the app’s page-based interface for the given scrolling orientation.

class func reloadRootControllers(withNamesAndContexts: [(name: String, context: AnyObject)])

Loads the specified interface controllers and rebuilds the app’s page-based interface.

func becomeCurrentPage()

Displays the interface controller in the page-based interface.

