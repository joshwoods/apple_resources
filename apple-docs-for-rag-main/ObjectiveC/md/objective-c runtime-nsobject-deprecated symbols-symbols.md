

- Objective-C Runtime
- NSObject
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review symbols that are no longer supported and find the replacements to use instead.

## Topics

### Deprecated Class Methods

class func defaultPlaceholder(for: Any?, with: NSBindingName) -> Any?

Returns an object that will be used as the placeholder for the `binding`, when a key value coding compliant property of an instance of the receiving class returns the value specified by `marker`, and no other placeholder has been specified.

Deprecated

class func setDefaultPlaceholder(Any?, for: Any?, with: NSBindingName)

Sets `placeholder` as the default placeholder for the `binding`, when a key value coding compliant property of an instance of the receiving class returns the value specified by `marker`, and no other placeholder has been specified.

Deprecated

class func useStoredAccessor() -> Bool

Returns `true` if the stored value methods storedValue(forKey:) and takeStoredValue(_:forKey:) should use private accessor methods in preference to public accessors.

Deprecated

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

func fileManager(FileManager, willProcessPath: String)

An `NSFileManager` object sends this message to a handler immediately before attempting to move, copy, rename, or delete, or before attempting to link to a given path.

Deprecated

func finalize()

The garbage collector invokes this method on the receiver before disposing of the memory it uses.

Deprecated

func fontManager(Any, willIncludeFont: String) -> Bool

Requests permission from the Font panel delegate to display the given font name in the Font panel.

Deprecated

func namesOfPromisedFilesDropped(atDestination: URL) -> [String]?

Returns the names of the files that the receiver promises to create at a specified location.

Deprecated

func storedValue(forKey: String) -> Any?

Returns the property identified by a given key.

Deprecated

func textStorageDidProcessEditing(Notification)Deprecated

func textStorageWillProcessEditing(Notification)Deprecated

func takeStoredValue(Any?, forKey: String)

Sets the value of the property identified by a given key.

Deprecated

func takeValue(Any?, forKey: String)

Sets the value for the property identified by `key` to `value`.

Deprecated

func takeValue(Any?, forKeyPath: String)

Sets the value for the property identified by `keyPath` to `value`.

Deprecated

func takeValues(from: [AnyHashable : Any])

Sets properties of the receiver with values from a given dictionary, using its keys to identify the properties

Deprecated

func unableToSetNil(forKey: String)

Invoked if `key` is represented by a scalar attribute.

Deprecated

func values(forKeys: [Any]) -> [AnyHashable : Any]

Returns a dictionary containing as keys the property names in `keys`, with corresponding values being the corresponding property values.

Deprecated

optional func workflowController(_ controller: AMWorkflowController, didError error: any Error)

Notifies the delegate when the workflow encounters an error.

optional func workflowController(_ controller: AMWorkflowController, didRun action: AMAction)

Notifies the delegate when the specified action finishes running.

optional func workflowController(_ controller: AMWorkflowController, willRun action: AMAction)

Notifies the delegate when the specified action is about to run.

optional func workflowControllerDidRun(_ controller: AMWorkflowController)

Notifies the delegate when the workflow controller object finishes running.

optional func workflowControllerDidStop(_ controller: AMWorkflowController)

Tells the delegate that the workflow controller object has stopped.

optional func workflowControllerWillRun(_ controller: AMWorkflowController)

Notifies the delegate when the workflow controller object is about to run.

optional func workflowControllerWillStop(_ controller: AMWorkflowController)

Tells the delegate that the workflow controller object is about to stop.

