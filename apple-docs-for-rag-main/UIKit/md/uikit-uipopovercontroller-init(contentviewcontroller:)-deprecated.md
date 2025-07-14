

- UIKit
- UIPopoverController
-  init(contentViewController:) Deprecated

Initializer

# init(contentViewController:)

Returns an initialized popover controller object.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
init(contentViewController viewController: UIViewController)
```

## Parameters 

`viewController`  

The view controller for managing the popover’s content. This parameter must not be `nil`.

## Return Value

An initialized popover controller object.

## Discussion

When initializing a popover controller, you must specify the view controller object whose content is to be displayed in the popover. You can change this view controller later by modifying the contentViewController property.

