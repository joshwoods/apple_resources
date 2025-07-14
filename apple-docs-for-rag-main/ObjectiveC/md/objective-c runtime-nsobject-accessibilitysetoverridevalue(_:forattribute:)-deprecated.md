

- Objective-C Runtime
- NSObject
-  accessibilitySetOverrideValue(\_:forAttribute:) Deprecated

Instance Method

# accessibilitySetOverrideValue(\_:forAttribute:)

Overrides the specified attribute in the receiver or adds it if it does not exist, and sets its value to the specified value.

macOS 10.1–10.10Deprecated

``` source
func accessibilitySetOverrideValue(
    _ value: Any?,
    forAttribute attribute: NSAccessibility.Attribute
) -> Bool
```

Deprecated

Use NSAccessibilityProtocol instead.

## Parameters 

`value`  

The attribute value to be set.

`attribute`  

The name of the attribute. See NSAccessibility constants for lists of attribute names.

## Return Value

YES if the override was successful; otherwise, NO.

## Discussion

This method is for changing the set of attributes on an instance, as an alternative to subclassing.

This method works only on objects whose class already implements the `NSAccessibility` protocol. If the specified attribute is already supported by the object, the value specified by this method wins.

If the specified attribute does not exist, it is created outside the `NSAccessibility` protocol, so `accessibilityAttributeNames` still returns the old list, which does not contain the new attribute. Likewise, `accessibilityAttributeValue` does not return attributes created by the override process nor does it return their overridden values.

The values of overridden attributes are not settable by accessibility clients.

If you need to undo the effect of using this method, call it again, passing `nil` for the value.

Ensure that you invoke this method on the actual object that represents the user interface element. For example, for `NSButton`, use the underlying `NSButtonCell` object. `NSButton` itself is ignored by accessibility.

This method works only on an object representing a single user interface element. So, for example, you cannot use it when a single object represents multiple user interface elements, as with `NSSegmentedCell`, which has only a single object but provides user interface elements for each segment.

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

func accessibilityIsIgnored() -> Bool

Returns a Boolean value indicating whether the receiver should be ignored in the parent-child accessibility hierarchy.

Deprecated

func accessibilityParameterizedAttributeNames() -> [NSAccessibility.ParameterizedAttribute]

Returns a list of parameterized attribute names supported by the receiver.

Deprecated

func accessibilityPerformAction(NSAccessibility.Action)

Performs the action associated with the specified action.

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

