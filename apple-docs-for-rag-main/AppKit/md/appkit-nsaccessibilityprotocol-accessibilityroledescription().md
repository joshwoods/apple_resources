

- AppKit
- NSAccessibilityProtocol
-  accessibilityRoleDescription() 

Instance Method

# accessibilityRoleDescription()

Returns a localized, human-intelligible description of the accessibility element’s role, such as *radio button*.

macOS 10.10+

``` source
func accessibilityRoleDescription() -> String?
```

**Required**

## See Also

### Assigning Roles

func isAccessibilityRequired() -> Bool

Returns a Boolean value that determines whether the accessibility element must have content for successful submission of a form.

**Required**

func setAccessibilityRequired(Bool)

Sets a Boolean value that determines whether the accessibility element must have content for successful submission of a form.

**Required**

func accessibilityRole() -> NSAccessibility.Role?

Returns the type of interface element that the accessibility element represents.

**Required**

func setAccessibilityRole(NSAccessibility.Role?)

Sets the type of interface element that the accessibility element represents.

**Required**

func setAccessibilityRoleDescription(String?)

Sets the localized, human-intelligible description of the accessibility element’s role, such as *radio button*.

**Required**

func accessibilitySubrole() -> NSAccessibility.Subrole?

Returns the specialized interface element type that the accessibility element represents.

**Required**

func setAccessibilitySubrole(NSAccessibility.Subrole?)

Sets the specialized interface element type that the accessibility element represents.

**Required**

struct Role

Values that describe types of objects that accessibility elements represent.

struct Subrole

Values that describe specialized object subtypes that accessibility elements represent.

