

- Objective-C Runtime
- NSObject
-  accessibilityIsAttributeSettable(\_:) Deprecated

Instance Method

# accessibilityIsAttributeSettable(\_:)

Returns a Boolean value that indicates whether the value for the specified attribute in the receiver can be set.

macOS 10.1–10.10Deprecated

``` source
func accessibilityIsAttributeSettable(_ attribute: NSAccessibility.Attribute) -> Bool
```

Deprecated

Use NSAccessibilityProtocol instead.

## Parameters 

`attribute`  

The name of the attribute. See NSAccessibility constants for lists of attribute names.

## Return Value

YES if the specified attribute can be set; otherwise, NO.

## Discussion

User interface classes must implement this method. Subclasses should invoke the superclass’s implementation, if it exists, if `attribute` is not implemented in the subclass.

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

func accessibilityIsIgnored() -> Bool

Returns a Boolean value indicating whether the receiver should be ignored in the parent-child accessibility hierarchy.

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

