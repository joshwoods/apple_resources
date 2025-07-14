

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXVisibleChildrenAttribute 

Global Variable

# kAXVisibleChildrenAttribute

macOS 10.2+

``` source
var kAXVisibleChildrenAttribute: String { get }
```

## Discussion

An array of first-order accessibility objects contained by this accessibility object that are visible to a sighted user. For example, a list view’s `AXVisibleChildren` array would contain the list’s subelements that are currently scrolled into view. The members of the `AXVisibleChildren` array are a subset of the members of this accessibility object’s `AXChildren` array. This attribute is recommended for accessibility objects whose child objects can be scrolled out of view or otherwise obscured.

