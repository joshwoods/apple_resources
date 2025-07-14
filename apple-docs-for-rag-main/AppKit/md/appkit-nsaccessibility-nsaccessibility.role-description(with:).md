

- AppKit
- NSAccessibility
- NSAccessibility.Role
-  description(with:) 

Instance Method

# description(with:)

Returns a standard description for a role and subrole.

macOS

``` source
func description(with subrole: NSAccessibility.Subrole?) -> String?
```

## Discussion

You should pass `nil` to this function if there is no subrole. This function returns a description of a standard role. For example, if you implement a button widget that does not inherit from NSButton, you should use this function to return a localized role description matching that returned by a standard button.

## See Also

### Descriptions

static func description(for: Any) -> String?

Returns a standard role description for a user interface element.

