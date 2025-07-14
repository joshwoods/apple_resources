

- AppKit
- NSAccessibility
- NSAccessibility.Role
-  description(for:) 

Type Method

# description(for:)

Returns a standard role description for a user interface element.

macOS

``` source
static func description(for element: Any) -> String?
```

## Discussion

This function is like the description(with:) function, except that it queries `element` to get the role and subrole. The description(with:) function is more efficient, but this function is useful for accessorizing base classes so that they properly handle derived classes, which may override the subrole or even the role.

## See Also

### Descriptions

func description(with: NSAccessibility.Subrole?) -> String?

Returns a standard description for a role and subrole.

