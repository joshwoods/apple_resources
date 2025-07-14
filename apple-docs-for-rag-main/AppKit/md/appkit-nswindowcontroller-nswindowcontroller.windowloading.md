

- AppKit
- NSWindowController
-  NSWindowController.WindowLoading 

Structure

# NSWindowController.WindowLoading

A property wrapper that loads the receiver’s window.

macOS 13.3+Swift 5.1+

``` source
@propertyWrapper
struct WindowLoading
```

## Overview

Use this property wrapper on window controller properties that can be `nil` before the window controller’s window loads. Wrapping window controller properties this way eliminates crashes that can occur from implicitly defining properties as Optional, and then referencing them before the window controller finishes loading.

The following example uses the `NSWindowController.WindowLoading` property wrapper to ensure that `dateLabel` NSTextField loads before referencing it in the `didSet` of the `date` property observer:

```
class DateWindowController: NSWindowController {
    @WindowLoading private var dateLabel: NSTextField

    var date: Date? {
        didSet {
            let dateFormatter = DateFormatter()
            dateFormatter.dateStyle = .full
            let dateString = dateFormatter.string(from: self.date ?? Date())
            self.dateLabel.stringValue = dateString
        }
    }
}
```

After loading NSTextField, the system can safely access and set the `date` property.

```
let dateWindowController = DateWindowController()
dateWindowController.date = Date()
```

Use this property wrapper over implicitly unwrapped optionals for `IBOutlets` as well.

```
@IBOutlet @WindowLoading private var dateLabel: NSTextField
```

## Topics

### Creating a WindowLoading Property Wrapper

init()

Creates an empty property wrapper that loads the window controller’s window before accessing the property.

init(wrappedValue: Value)

Creates a property wrapper that loads the window controller’s window before accessing the property.

## See Also

### Related Documentation

struct ViewLoading

A property wrapper that loads the view controller’s view before accessing the property.

