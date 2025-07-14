

- Objective-C Runtime
- NSObject
-  storedValue(forKey:) Deprecated

Instance Method

# storedValue(forKey:)

Returns the property identified by a given key.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func storedValue(forKey key: String) -> Any?
```

Deprecated

If you are using the `NSManagedObject` class, use primitiveValue(forKey:) instead.

## Discussion

This method is used when the value is retrieved for storage in an object store (generally, this storage is ultimately in a database) or for inclusion in a snapshot. The default implementation is similar to the implementation of value(forKey:), but it resolves `key` with a different method/instance variable search order:

1.  Searches for a private accessor method based on `key` (a method preceded by an underbar). For example, with a `key` of “lastName”, storedValue(forKey:) looks for a method named `_getLastName` or `_lastName`.

2.  If a private accessor is not found, searches for an instance variable based on `key` and returns its value directly. For example, with a `key` of “lastName”, storedValue(forKey:) looks for an instance variable named `_lastName` or `lastName`.

3.  If neither a private accessor nor an instance variable is found, storedValue(forKey:) searches for a public accessor method based on `key`. For the `key` “lastName”, this would be `getLastName` or `lastName`.

4.  If `key` is unknown, storedValue(forKey:) calls handleTakeValue(_:forUnboundKey:).

This different search order allows an object to bypass processing that is performed before returning a value through a public API. However, if you always want to use the search order in value(forKey:), you can implement the class method useStoredAccessor() to return NO. And as with value(forKey:), you can prevent direct access of an instance variable with the class method accessInstanceVariablesDirectly.

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

func accessibilitySetOverrideValue(Any?, forAttribute: NSAccessibility.Attribute) -> Bool

Overrides the specified attribute in the receiver or adds it if it does not exist, and sets its value to the specified value.

Deprecated

func accessibilitySetValue(Any?, forAttribute: NSAccessibility.Attribute)

Sets the value of the specified attribute in the receiver to the specified value.

Deprecated

func fileManager(FileManager, shouldProceedAfterError: [AnyHashable : Any]) -> Bool

An `NSFileManager` object sends this message to its handler for each error it encounters when copying, moving, removing, or linking files or directories.

Deprecated

