

- UIKit
- UIMenuItem
-  init(title:action:) Deprecated

Initializer

# init(title:action:)

Creates and returns a menu-item object initialized with the given title and action.

iOS 3.2–16.0DeprecatediPadOS 3.2–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
init(
    title: String,
    action: Selector
)
```

## Parameters 

`title`  

The title of the menu item.

`action`  

A selector identifying the method of the responder object to invoke for handling the command represented by the menu item.

## Return Value

An initialized `UIMenuItem` object, or `nil` if there was a problem creating the object.

