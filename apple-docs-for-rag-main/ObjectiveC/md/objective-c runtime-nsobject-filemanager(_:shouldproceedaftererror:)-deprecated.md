

- Objective-C Runtime
- NSObject
-  fileManager(\_:shouldProceedAfterError:) Deprecated

Instance Method

# fileManager(\_:shouldProceedAfterError:)

An `NSFileManager` object sends this message to its handler for each error it encounters when copying, moving, removing, or linking files or directories.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func fileManager(
    _ fm: FileManager,
    shouldProceedAfterError errorInfo: [AnyHashable : Any]
) -> Bool
```

Deprecated

See delegate methods for copy, move, remove, and link methods.

## Parameters 

`fm`  

The file manager that sent this message.

`errorInfo`  

A dictionary that contains two or three pieces of information (all NSString objects) related to the error:

| Key         | Value                                                   |
|-------------|---------------------------------------------------------|
| `@"Path"`   | The path related to the error (usually the source path) |
| `@"Error"`  | A description of the error                              |
| `@"ToPath"` | The destination path (not all errors)                   |

## Return Value

YES if the operation (which is often continuous within a loop) should proceed, otherwise NO.

## Discussion

An `NSFileManager` object, `manager`, sends this message for each error it encounters when copying, moving, removing, or linking files or directories. The return value is passed back to the invoker of copyPath:toPath:handler:, movePath:toPath:handler:, removeFileAtPath:handler:, or linkPath:toPath:handler:. If an error occurs and your handler has not implemented this method, the invoking method automatically returns NO.

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

func fileManager(FileManager, willProcessPath: String)

An `NSFileManager` object sends this message to a handler immediately before attempting to move, copy, rename, or delete, or before attempting to link to a given path.

Deprecated

