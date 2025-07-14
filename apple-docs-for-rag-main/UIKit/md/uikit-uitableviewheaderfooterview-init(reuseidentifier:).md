

- UIKit
- UITableViewHeaderFooterView
-  init(reuseIdentifier:) 

Initializer

# init(reuseIdentifier:)

Initializes a header-footer view with the specified reuse identifier.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(reuseIdentifier: String?)
```

## Parameters 

`reuseIdentifier`  

A string used to identify the header or footer view if it’s to be reused by multiple sections. Pass `nil` if the view isn’t to be reused. You should use the same reuse identifier for all header or footer views of the same form.

## Return Value

An initialized UITableViewHeaderFooterView object or `nil` if the object could not be created.

## Discussion

Once set, you can’t change the reuse identifier for the returned view object.

## See Also

### Creating the view

init?(coder: NSCoder)

Creates a header-footer view from data in an unarchiver.

