

- UIKit
- UIViewController
-  UIViewController.ViewLoading 

Structure

# UIViewController.ViewLoading

A property wrapper that loads the view controller’s view before accessing the property.

iOS 16.4+iPadOS 16.4+Mac CatalysttvOS 16.4+visionOSSwift 5.1+

``` source
@propertyWrapper
struct ViewLoading
```

## Overview

Use this property wrapper on view controller properties that can be `nil` before the view controller’s view loads. Wrapping view controller properties this way eliminates crashes that can occur from implicitly defining properties as Optional, and then referencing them before the view controller finishes loading.

The following example uses the UIViewController.ViewLoading wrapper to ensure that `dateLabel` UILabel loads before referencing it in the `didSet` of the `date` property observer:

```
class DateViewController: UIViewController {
    @ViewLoading private var dateLabel: UILabel

    var date: Date? {
        didSet {
            let dateFormatter = DateFormatter()
            dateFormatter.dateStyle = .full
            let dateString = dateFormatter.string(from: self.date ?? Date())
            // If the view controller's view hasn't loaded yet,
            // accessing the dateLabel property here causes it to load.
            self.dateLabel.text = dateString
        }
    }

    override func viewDidLoad() {
        super.viewDidLoad()
        let label = UILabel(frame: self.view.bounds)
        self.view.addSubview(label)
        self.dateLabel = label
    }
}
```

After loading UILabel, the system can safely access and set the `date` property.

```
let dateViewController = DateViewController()
dateViewController.date = Date()
```

Use this property wrapper over implicitly unwrapped optionals for `IBOutlets` as well.

```
@IBOutlet @ViewLoading private var dateLabel: UILabel
```

## Topics

### Creating a ViewLoading property wrapper

init()

Creates an empty property wrapper that loads the view controller’s view before accessing the property.

init(wrappedValue: Value)

Creates a property wrapper that loads the view controller’s view before accessing the property.

## See Also

### Supporting types

enum UIContainerBackgroundStyle

