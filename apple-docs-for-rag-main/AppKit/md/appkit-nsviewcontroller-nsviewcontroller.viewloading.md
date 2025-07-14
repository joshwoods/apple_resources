

- AppKit
- NSViewController
-  NSViewController.ViewLoading 

Structure

# NSViewController.ViewLoading

A property wrapper that loads the view controller’s view before accessing the property.

macOS 13.3+Swift 5.1+

``` source
@propertyWrapper
struct ViewLoading
```

## Overview

Use this property wrapper on view controller properties that can be `nil` before the view controller’s view loads. Wrapping view controller properties this way eliminates crashes that can occur from implicitly defining properties as Optional, and then referencing them before the view controller finishes loading.

The following example uses the `NSViewController.ViewLoading` wrapper to ensure that `dateLabel` NSTextField loads before referencing it in the `didSet` of the `date` property observer:

```
class DateViewController: NSViewController {
    @ViewLoading private var dateLabel: NSTextField

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
let dateViewController = DateViewController()
dateViewController.date = Date()
```

Use this property wrapper over implicitly unwrapped optionals for `IBOutlets` as well.

```
@IBOutlet @ViewLoading private var dateLabel: NSTextField
```

## Topics

### Creating a ViewLoading Property Wrapper

init()

Creates an empty property wrapper that loads the view controller’s view before accessing the property.

init(wrappedValue: Value)

Creates a property wrapper that loads the view controller’s view before accessing the property.

## See Also

### Related Documentation

struct WindowLoading

A property wrapper that loads the receiver’s window.

