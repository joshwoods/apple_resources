

- AppKit
- NSMenuItem
-  init(title:action:keyEquivalent:) 

Initializer

# init(title:action:keyEquivalent:)

Returns an initialized instance of `NSMenuItem`.

macOS

``` source
init(
    title string: String,
    action selector: Selector?,
    keyEquivalent charCode: String
)
```

## Parameters 

`string`  

The title of the menu item. This value must not be `nil` (if there is no title, specify an empty `NSString`).

`selector`  

The action selector to be associated with the menu item. This value must be a valid selector or `NULL`.

`charCode`  

A string representing a keyboard key to be used as the key equivalent. This value must not be `nil` (if there is no key equivalent, specify an empty `NSString`).

## Return Value

An instance of `NSMenuItem`.

## Discussion

For instances of the `NSMenuItem` class, the default initial state is `NSOffState`, the default on-state image is a check mark, and the default mixed-state image is a dash.

## See Also

### Related Documentation

Application Menu and Pop-up List Programming Topics

### Creating a menu item

init(coder: NSCoder)

