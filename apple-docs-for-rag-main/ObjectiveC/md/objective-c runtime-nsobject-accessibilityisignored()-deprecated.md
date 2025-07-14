

- Objective-C Runtime
- NSObject
-  accessibilityIsIgnored() Deprecated

Instance Method

# accessibilityIsIgnored()

Returns a Boolean value indicating whether the receiver should be ignored in the parent-child accessibility hierarchy.

macOS 10.1–10.10Deprecated

``` source
func accessibilityIsIgnored() -> Bool
```

Deprecated

Use NSAccessibilityProtocol instead.

## Return Value

YES if the receiver should be ignored; otherwise, NO.

## Discussion

When asking for an object’s children, do not include ignored children; instead, replace the ignored children with their own unignored children. The same applies when asking for an object’s parent: skip the ignored parent and treat the first unignored ancestor as the real parent. Likewise, when a hit-test or focus test is satisfied by an ignored element, use the element’s first unignored ancestor (or descendant in certain cases, such as single-celled controls) instead.

Ignored elements let you provide a simplified version of the view and object ownership hierarchies. Accessibility clients can bypass intermediate objects, letting users access the real user interface objects more quickly. For example, `NSControl` objects are ignored when they are single-celled; the visible parent-child relationship is between the control’s parent (or a higher ancestor if the parent is ignored, too) and the control’s cell.

## See Also

### Deprecated Methods

func accessibilityAttributeNames() -> [NSAccessibility.Attribute]

Returns an array of attribute names supported by the receiver.

Deprecated

func accessibilityAttributeValue(NSAccessibility.Attribute) -> Any?

Returns the value of the specified attribute in the receiver.

Deprecated

func accessibilityAttributeValue(NSAccessibility.ParameterizedAttribute, forParameter: Any?) -> Any?

Returns the value of the receiver’s parameterized attribute corresponding to the specified attribute name and parameter.

Deprecated

func accessibilityActionDescription(NSAccessibility.Action) -> String?

Returns a localized description of the specified action.

Deprecated

func accessibilityActionNames() -> [NSAccessibility.Action]

Returns an array of action names supported by the accessibility element.

Deprecated

func accessibilityArrayAttributeCount(NSAccessibility.Attribute) -> Int

Returns the count of the specified accessibility array attribute.

Deprecated

func accessibilityArrayAttributeValues(NSAccessibility.Attribute, index: Int, maxCount: Int) -> [Any]

Returns a subarray of values of an accessibility array attribute.

Deprecated

func accessibilityIndex(ofChild: Any) -> Int

Returns the index of the specified accessibility child in the parent.

Deprecated

func accessibilityIsAttributeSettable(NSAccessibility.Attribute) -> Bool

Returns a Boolean value that indicates whether the value for the specified attribute in the receiver can be set.

Deprecated

func accessibilityParameterizedAttributeNames() -> [NSAccessibility.ParameterizedAttribute]

Returns a list of parameterized attribute names supported by the receiver.

Deprecated

func accessibilityPerformAction(NSAccessibility.Action)

Performs the action associated with the specified action.

Deprecated

func accessibilitySetOverrideValue(Any?, forAttribute: NSAccessibility.Attribute) -> Bool

Overrides the specified attribute in the receiver or adds it if it does not exist, and sets its value to the specified value.

Deprecated

func accessibilitySetValue(Any?, forAttribute: NSAccessibility.Attribute)

Sets the value of the specified attribute in the receiver to the specified value.

Deprecated

func fileManager(FileManager, shouldProceedAfterError: [AnyHashable : Any]) -> Bool

An `NSFileManager` object sends this message to its handler for each error it encounters when copying, moving, removing, or linking files or directories.

Deprecated

func fileManager(FileManager, willProcessPath: String)

An `NSFileManager` object sends this message to a handler immediately before attempting to move, copy, rename, or delete, or before attempting to link to a given path.

Deprecated

