

- AppKit
- NSAccessibilityElement
-  element(withRole:frame:label:parent:) 

Type Method

# element(withRole:frame:label:parent:)

Instantiates and configures a new accessibility element.

macOS 10.10+

``` source
class func element(
    withRole role: NSAccessibility.Role,
    frame: NSRect,
    label: String?,
    parent: Any?
) -> Any
```

## Parameters 

`role`  

The new element’s intended role. For a complete list of roles, see Roles.

Note

Your subclass also needs to adopt the role-based protocol that corresponds with this role.

`frame`  

The element’s frame in screen coordinates. Additionally, you need to set the element’s accessibilityFrameInParentSpace property.

Note

The accessibilityFrameInParentSpace property ensures that the element’s frame is updated as its parent moves.

`label`  

A short description of the new element. Do not include the element’s type in the label (for example, use `Play`, not `Play button`). If possible, use a single word. To help ensure that accessibility clients such as VoiceOver read the label with the correct intonation, start the label with a capital letter. Do not put a period at the end. Always localize the label.

`parent`  

The new element’s parent in the accessibility hierarchy.

## Return Value

A newly instantiated and initialized accessibility element.

## Discussion

Alternatively, instead of calling this convenience method, you can create an accessibility element and set its accessibilityRole, accessibilityLabel, and accessibilityParent properties. Regardless of how you create the accessibility element, you need to set its accessibilityFrameInParentSpace property to ensure that the element’s frame is updated as its parent moves.

## See Also

### Supporting the Accessibility Hierarchy

func accessibilityAddChildElement(NSAccessibilityElement)

Adds a child to the accessibility element in the accessibility hierarchy.

func accessibilityFrameInParentSpace() -> NSRect

Returns the accessibility element’s frame in its parent’s coordinate system.

func setAccessibilityFrameInParentSpace(NSRect)

Sets the accessibility element’s frame in its parent’s coordinate system.

