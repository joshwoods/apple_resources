

- Quartz
-  QuartzFilterManager 

Class

# QuartzFilterManager

macOS 10.4+

``` source
class QuartzFilterManager
```

## Topics

### Instance Methods

func delegate() -> Any!

func filterPanel() -> NSPanel!

func filterView() -> QuartzFilterView!

func importFilter([AnyHashable : Any]!) -> QuartzFilter!

func select(QuartzFilter!) -> Bool

func selectedFilter() -> QuartzFilter!

func setDelegate(Any!)

### Type Methods

class func filters(inDomains: [Any]!) -> [Any]!

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

### Classes

class QuartzFilter

class QuartzFilterView

