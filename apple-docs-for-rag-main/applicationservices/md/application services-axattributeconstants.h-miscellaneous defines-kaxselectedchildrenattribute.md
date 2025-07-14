

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXSelectedChildrenAttribute 

Global Variable

# kAXSelectedChildrenAttribute

macOS 10.2+

``` source
var kAXSelectedChildrenAttribute: String { get }
```

## Discussion

An array of selected first-order accessibility objects contained by this accessibility object. For example, the selected subelements of a list view are contained in the `AXSelectedChildren` array of the list view’s accessibility object. The members of the `AXSelectedChildren` array are a subset of the members of this accessibility object’s `AXChildren` array. This attribute is required for accessibility objects that contain selectable child objects.

