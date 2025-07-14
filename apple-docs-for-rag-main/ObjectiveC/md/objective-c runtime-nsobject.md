

- Objective-C Runtime
-  NSObject 

Class

# NSObject

The root class of most Objective-C class hierarchies, from which subclasses inherit a basic interface to the runtime system and the ability to behave as Objective-C objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class NSObject
```

## Topics

### Initializing a Class

class func initialize()

Initializes the class before it receives its first message.

class func load()

Invoked whenever a class or category is added to the Objective-C runtime; implement this method to perform class-specific behavior upon loading.

### Creating, Copying, and Deallocating Objects

init()

Implemented by subclasses to initialize a new object (the receiver) immediately after memory for it has been allocated.

func copy() -> Any

Returns the object returned by `copy(with:)`.

func mutableCopy() -> Any

Returns the object returned by `mutableCopy(with:)` where the zone is `nil`.

### Identifying Classes

class func superclass() -> AnyClass?

Returns the class object for the receiver’s superclass.

class func isSubclass(of: AnyClass) -> Bool

Returns a Boolean value that indicates whether the receiving class is a subclass of, or identical to, a given class.

### Testing Class Functionality

class func instancesRespond(to: Selector!) -> Bool

Returns a Boolean value that indicates whether instances of the receiver are capable of responding to a given selector.

### Testing Protocol Conformance

class func conforms(to: Protocol) -> Bool

Returns a Boolean value that indicates whether the target conforms to a given protocol.

### Obtaining Information About Methods

func method(for: Selector!) -> IMP!

Locates and returns the address of the receiver’s implementation of a method so it can be called as a function.

class func instanceMethod(for: Selector!) -> IMP!

Locates and returns the address of the implementation of the instance method identified by a given selector.

### Describing Objects

class func description() -> String

Returns a string that represents the contents of the receiving class.

### Supporting Discardable Content

var autoContentAccessingProxy: Any

A proxy for the receiving object

### Sending Messages

func perform(Selector, with: Any?, afterDelay: TimeInterval)

Invokes a method of the receiver on the current thread using the default mode after a delay.

func perform(Selector, with: Any?, afterDelay: TimeInterval, inModes: [RunLoop.Mode])

Invokes a method of the receiver on the current thread using the specified modes after a delay.

func performSelector(onMainThread: Selector, with: Any?, waitUntilDone: Bool)

Invokes a method of the receiver on the main thread using the default mode.

func performSelector(onMainThread: Selector, with: Any?, waitUntilDone: Bool, modes: [String]?)

Invokes a method of the receiver on the main thread using the specified modes.

func perform(Selector, on: Thread, with: Any?, waitUntilDone: Bool)

Invokes a method of the receiver on the specified thread using the default mode.

func perform(Selector, on: Thread, with: Any?, waitUntilDone: Bool, modes: [String]?)

Invokes a method of the receiver on the specified thread using the specified modes.

func performSelector(inBackground: Selector, with: Any?)

Invokes a method of the receiver on a new background thread.

class func cancelPreviousPerformRequests(withTarget: Any)

Cancels perform requests previously registered with the perform(_:with:afterDelay:) instance method.

class func cancelPreviousPerformRequests(withTarget: Any, selector: Selector, object: Any?)

Cancels perform requests previously registered with perform(_:with:afterDelay:).

### Forwarding Messages

func forwardingTarget(for: Selector!) -> Any?

Returns the object to which unrecognized messages should first be directed.

### Dynamically Resolving Methods

class func resolveClassMethod(Selector!) -> Bool

Dynamically provides an implementation for a given selector for a class method.

class func resolveInstanceMethod(Selector!) -> Bool

Dynamically provides an implementation for a given selector for an instance method.

### Handling Errors

func doesNotRecognizeSelector(Selector!)

Handles messages the receiver doesn’t recognize.

### Archiving

func awakeAfter(using: NSCoder) -> Any?

Overridden by subclasses to substitute another object in place of the object that was decoded and subsequently received this message.

var classForArchiver: AnyClass?

The class to substitute for the receiver’s own class during archiving.

var classForCoder: AnyClass

Overridden by subclasses to substitute a class other than its own during coding.

var classForKeyedArchiver: AnyClass?

Subclasses to substitute a new class for instances during keyed archiving.

class func classFallbacksForKeyedArchiver() -> [String]

Overridden to return the names of classes that can be used to decode objects if their class is unavailable.

class func classForKeyedUnarchiver() -> AnyClass

Overridden by subclasses to substitute a new class during keyed unarchiving.

func replacementObject(for: NSArchiver) -> Any?

Overridden by subclasses to substitute another object for itself during archiving.

Deprecated

func replacementObject(for: NSCoder) -> Any?

Overridden by subclasses to substitute another object for itself during encoding.

func replacementObject(for: NSKeyedArchiver) -> Any?

Overridden by subclasses to substitute another object for itself during keyed archiving.

class func setVersion(Int)

Sets the receiver’s version number.

class func version() -> Int

Returns the version number assigned to the class.

### Working with Class Descriptions

var attributeKeys: [String]

An array of `NSString` objects containing the names of immutable values that instances of the receiver’s class contain.

var classDescription: NSClassDescription

An object containing information about the attributes and relationships of the receiver’s class.

func inverse(forRelationshipKey: String) -> String?

For a given key that defines the name of the relationship from the receiver’s class to another class, returns the name of the relationship from the other class to the receiver’s class.

var toManyRelationshipKeys: [String]

An array containing the keys for the to-many relationship properties of the receiver.

var toOneRelationshipKeys: [String]

The keys for the to-one relationship properties of the receiver, if any.

### Improving Accessibility

UIAccessibility

A set of methods that provides accessibility information about views and controls in an app’s user interface.

UIAccessibilityContainer

Provide a set of methods that view subclasses use to make subcomponents accessible as separate elements.

UIAccessibilityAction

A set of methods that accessibility elements can use to support specific actions.

UIAccessibilityFocus

An informal protocol that provides a way to determine whether an assistive app, such as VoiceOver, has focus on an accessible element.

UIAccessibilityDragging

A pair of properties to allow you to fine-tune how drags and drops are exposed to assistive technologies.

### Improving browser accessibility

func browserAccessibilityAttributedValue(in: NSRange) -> NSAttributedString

Returns the value for this element within the given range, as an attributed string.

func browserAccessibilityDeleteTextAtCursor(numberOfCharacters: Int)

Deletes text from the element at the current cursor position.

func browserAccessibilityInsertTextAtCursor(text: String)

Inserts text into the element at the current cursor position.

func browserAccessibilitySelectedTextRange() -> NSRange

Returns the range of selected text in the element.

func browserAccessibilitySetSelectedTextRange(NSRange)

Updates the element’s selected text.

func browserAccessibilityValue(in: NSRange) -> String

Returns this element’s value in the given range.

var browserAccessibilityContainerType: BEAccessibilityContainerType

The kind of container that contains this element.

var browserAccessibilityCurrentStatus: String?

A string that’s the element’s value for aria-current.

var browserAccessibilityHasDOMFocus: Bool

A Boolean value that indicates whether the element has native focus in the browser Document Object Model.

var browserAccessibilityIsRequired: Bool

A Boolean value that’s the element’s value for aria-required.

var browserAccessibilityPressedState: BEAccessibilityPressedState

The element’s value for aria-pressed.

var browserAccessibilityRoleDescription: String?

A string that describes the element’s role for assistive technologies.

var browserAccessibilitySortDirection: String?

A string that’s the element’s value for aria-sort.

### Scripting

var classCode: FourCharCode

The receiver’s Apple event type code, as stored in the `NSScriptClassDescription` object for the object’s class.

var className: String

A string containing the name of the class.

func copyScriptingValue(Any, forKey: String, withProperties: [String : Any]) -> Any?

Creates and returns one or more scripting objects to be inserted into the specified relationship by copying the passed-in value and setting the properties in the copied object or objects.

func newScriptingObject(of: AnyClass, forValueForKey: String, withContentsValue: Any?, properties: [String : Any]) -> Any?

Creates and returns an instance of a scriptable class, setting its contents and properties, for insertion into the relationship identified by the key.

var scriptingProperties: [String : Any]?

An `NSString`-keyed dictionary of the receiver’s scriptable properties.

func scriptingValue(for: NSScriptObjectSpecifier) -> Any?

Given an object specifier, returns the specified object or objects in the receiving container.

### Integrating with Combine

struct KeyValueObservingPublisher

A Combine publisher that produces a new element whenever the observed value changes.

### Key-Value Observing

NSKeyValueObserving

An informal protocol that objects adopt to be notified of changes to the specified properties of other objects.

### Key-Value Coding

NSKeyValueBindingCreation

A set of methods that you can use to create and remove bindings between view objects and controllers, or between controllers and model objects.

NSKeyValueCoding

A mechanism by which you can access the properties of an object indirectly by name or key.

NSScriptKeyValueCoding

A collection of methods that provide additional capabilities for working with key-value coding.

NSScriptKeyValueCoding Exception Names

Exceptions raised by key-value coding methods.

### Interacting with Web Plug-ins

WebPlugInContainer

`WebPlugInContainer` is an informal protocol that enables a plug-in to send messages to the application.

WebPlugIn

The `WebPlugIn` informal protocol defines methods that enable interaction between an application using the WebKit framework and any WebKit-based plug-ins it may use.

### Implementing Web Scripting

WebScripting

`WebScripting` is an informal protocol that defines methods that classes can implement to export their interfaces to a WebScript environment such as JavaScript.

### Supporting Cocoa Scripting

NSScriptingComparisonMethods

A collection of methods useful for comparing script objects.

### Deprecated

Avoid using deprecated classes and protocols in your apps.

Deprecated Symbols

Review symbols that are no longer supported and find the replacements to use instead.

### Instance Properties

var accessibilityActivateBlock: AXBoolReturnBlock?

var accessibilityActivationPoint: CGPoint

var accessibilityActivationPointBlock: AXPointReturnBlock?

var accessibilityAttributedHint: NSAttributedString?

var accessibilityAttributedHintBlock: AXAttributedStringReturnBlock?

var accessibilityAttributedLabel: NSAttributedString?

var accessibilityAttributedLabelBlock: AXAttributedStringReturnBlock?

var accessibilityAttributedUserInputLabels: [NSAttributedString]!

var accessibilityAttributedUserInputLabelsBlock: AXAttributedStringArrayReturnBlock?

var accessibilityAttributedValue: NSAttributedString?

var accessibilityAttributedValueBlock: AXAttributedStringReturnBlock?

var accessibilityContainerType: UIAccessibilityContainerType

var accessibilityContainerTypeBlock: AXContainerTypeReturnBlock?

var accessibilityCustomActionsBlock: AXCustomActionsReturnBlock?

var accessibilityCustomRotors: [UIAccessibilityCustomRotor]?

var accessibilityCustomRotorsBlock: AXCustomRotorsReturnBlock?

var accessibilityDecrementBlock: AXVoidReturnBlock?

var accessibilityDirectTouchOptions: UIAccessibility.DirectTouchOptions

var accessibilityElements: [Any]?

var accessibilityElementsBlock: AXArrayReturnBlock?

var accessibilityElementsHidden: Bool

var accessibilityElementsHiddenBlock: AXBoolReturnBlock?

var accessibilityExpandedStatus: UIAccessibility.ExpandedStatus

var accessibilityExpandedStatusBlock: (() -> UIAccessibility.ExpandedStatus)?

var accessibilityFocusedUIElement: Any?

var accessibilityFrame: CGRect

var accessibilityFrameBlock: AXRectReturnBlock?

var accessibilityHeaderElements: [Any]?

var accessibilityHeaderElementsBlock: AXArrayReturnBlock?

var accessibilityHint: String?

var accessibilityHintBlock: AXStringReturnBlock?

var accessibilityIdentifierBlock: AXStringReturnBlock?

var accessibilityIncrementBlock: AXVoidReturnBlock?

var accessibilityLabel: String?

var accessibilityLabelBlock: AXStringReturnBlock?

var accessibilityLanguage: String?

var accessibilityLanguageBlock: AXStringReturnBlock?

var accessibilityMagicTapBlock: AXBoolReturnBlock?

var accessibilityNavigationStyle: UIAccessibilityNavigationStyle

var accessibilityNavigationStyleBlock: AXNavigationStyleReturnBlock?

var accessibilityNextTextNavigationElement: Any?

var accessibilityNextTextNavigationElementBlock: AXObjectReturnBlock?

var accessibilityNotifiesWhenDestroyed: Bool

A Boolean value that indicates whether a custom accessibility object sends a notification when its corresponding UI element is destroyed.

var accessibilityPath: UIBezierPath?

var accessibilityPathBlock: AXPathReturnBlock?

var accessibilityPerformEscapeBlock: AXBoolReturnBlock?

var accessibilityPreviousTextNavigationElement: Any?

var accessibilityPreviousTextNavigationElementBlock: AXObjectReturnBlock?

var accessibilityRespondsToUserInteraction: Bool

var accessibilityRespondsToUserInteractionBlock: AXBoolReturnBlock?

var accessibilityShouldGroupAccessibilityChildrenBlock: AXBoolReturnBlock?

var accessibilityTextInputResponder: (any UITextInput)?

var accessibilityTextInputResponderBlock: AXUITextInputReturnBlock?

var accessibilityTextualContext: UIAccessibilityTextualContext?

var accessibilityTextualContextBlock: AXTextualContextReturnBlock?

var accessibilityTraits: UIAccessibilityTraits

var accessibilityTraitsBlock: AXTraitsReturnBlock?

var accessibilityUserInputLabels: [String]!

var accessibilityUserInputLabelsBlock: AXStringArrayReturnBlock?

var accessibilityValue: String?

var accessibilityValueBlock: AXStringReturnBlock?

var accessibilityViewIsModal: Bool

var accessibilityViewIsModalBlock: AXBoolReturnBlock?

var automationElements: [Any]?

var automationElementsBlock: AXArrayReturnBlock?

var isAccessibilityElement: Bool

var isAccessibilityElementBlock: AXBoolReturnBlock?

var isSelectable: Bool

var objectSpecifier: NSScriptObjectSpecifier?

Returns an object specifier for the receiver.

var shouldGroupAccessibilityChildren: Bool

### Instance Methods

func acceptsPreviewPanelControl(QLPreviewPanel!) -> Bool

func accessibilityElement(at: Int) -> Any?

func accessibilityElementCount() -> Int

func accessibilityHitTest(NSPoint) -> Any?

func accessibilityHitTest(CGPoint, event: UIEvent?) -> Any?

func accessibilityLineEndPositionFromCurrentSelection() -> Int

func accessibilityLineRange(forPosition: Int) -> NSRange

func accessibilityLineStartPositionFromCurrentSelection() -> Int

func accessibilityZoomIn(at: CGPoint) -> Bool

Zooms in on the content at the specified point.

func accessibilityZoomOut(at: CGPoint) -> Bool

Zooms out from the content at the specified point.

func actionProperty() -> String!

Sent to the delegate to request the property the action applies to.

func attemptRecovery(fromError: any Error, optionIndex: Int) -> Bool

Implemented to attempt a recovery from an error noted in an application-modal dialog.

func attemptRecovery(fromError: any Error, optionIndex: Int, delegate: Any?, didRecoverSelector: Selector?, contextInfo: UnsafeMutableRawPointer?)

Implemented to attempt a recovery from an error noted in a document-modal sheet.

func authorizationViewCreatedAuthorization(SFAuthorizationView!)

Sent to the delegate to indicate the authorization object has been created or changed.

func authorizationViewDidAuthorize(SFAuthorizationView!)

Sent to the delegate to indicate the user was authorized and the authorization view was changed to unlocked.

func authorizationViewDidDeauthorize(SFAuthorizationView!)

Sent to the delegate to indicate the user was deauthorized and the authorization view was changed to locked.

func authorizationViewDidHide(SFAuthorizationView!)

Sent to the delegate to indicate that the view’s visibility has changed.

func authorizationViewReleasedAuthorization(SFAuthorizationView!)

Sent to the delegate to indicate that deauthorization is about to occur.

func authorizationViewShouldDeauthorize(SFAuthorizationView!) -> Bool

Sent to the delegate when a user clicks the open lock icon.

func awakeFromNib()

Prepares the receiver for service after it has been loaded from an Interface Builder archive, or nib file.

func beginPreviewPanelControl(QLPreviewPanel!)

func burnProgressPanel(DRBurnProgressPanel!, burnDidFinish: DRBurn!) -> Bool

Allows the delegate to handle the end-of-burn feedback.

func burnProgressPanelDidFinish(Notification!)

Notification sent by the panel after ordering out.

func burnProgressPanelWillBegin(Notification!)

Notification sent by the panel before display.

func candidates(Any!) -> [Any]!

Returns an array of candidates.

func certificatePanelShowHelp(SFCertificatePanel!) -> Bool

Implements custom help behavior for the modal panel.

func chooseIdentityPanelShowHelp(SFChooseIdentityPanel!) -> Bool

Implements custom help behavior for the modal panel.

func commitComposition(Any!)

Informs the controller that the composition should be committed.

func composedString(Any!) -> Any!

Return the current composed string.

func compositionParameterView(QCCompositionParameterView!, didChangeParameterWithKey: String!)

Called after an input parameter in the composition parameter view has been edited.

Deprecated

func compositionParameterView(QCCompositionParameterView!, shouldDisplayParameterWithKey: String!, attributes: [AnyHashable : Any]!) -> Bool

Allows you to define which composition parameters are visible in the user interface when the composition parameter view refreshes.

Deprecated

func compositionPickerView(QCCompositionPickerView!, didSelect: QCComposition!)

Performs custom tasks when the selected composition in the composition picker view changes.

Deprecated

func compositionPickerViewDidStartAnimating(QCCompositionPickerView!)

Performs custom tasks when the composition picker view starts animating a composition.

Deprecated

func compositionPickerViewWillStopAnimating(QCCompositionPickerView!)

Performs custom tasks when the composition picker view stops animating a composition.

Deprecated

func didCommand(by: Selector!, client: Any!) -> Bool

Processes a command generated by user action such as typing certain keys or pressing the mouse button.

func doesContain(Any) -> Bool

Returns a Boolean value that indicates whether the receiver contains a given object.

func endPreviewPanelControl(QLPreviewPanel!)

func eraseProgressPanel(DREraseProgressPanel!, eraseDidFinish: DRErase!) -> Bool

Notification sent by the panel before display.

func eraseProgressPanelDidFinish(Notification!)

Notification sent by the panel after ordering out.

func eraseProgressPanelWillBegin(Notification!)

Notification sent by the panel before display.

func exceptionHandler(NSExceptionHandler!, shouldHandle: NSException!, mask: Int) -> Bool

Implemented by the delegate to evaluate whether the delegating exception handler should handle a given exception.

func exceptionHandler(NSExceptionHandler!, shouldLogException: NSException!, mask: Int) -> Bool

Implemented by the delegate to evaluate whether the delegating exception hangler should log a given exception.

func fileTransferServicesAbortComplete(OBEXFileTransferServices!, error: OBEXError)

func fileTransferServicesConnectionComplete(OBEXFileTransferServices!, error: OBEXError)

func fileTransferServicesCopyRemoteFileComplete(OBEXFileTransferServices!, error: OBEXError)

func fileTransferServicesCopyRemoteFileProgress(OBEXFileTransferServices!, transferProgress: [AnyHashable : Any]!)

func fileTransferServicesCreateFolderComplete(OBEXFileTransferServices!, error: OBEXError, folder: String!)

func fileTransferServicesDisconnectionComplete(OBEXFileTransferServices!, error: OBEXError)

func fileTransferServicesFilePreparationComplete(OBEXFileTransferServices!, error: OBEXError)

func fileTransferServicesPathChangeComplete(OBEXFileTransferServices!, error: OBEXError, finalPath: String!)

func fileTransferServicesRemoveItemComplete(OBEXFileTransferServices!, error: OBEXError, removedItem: String!)

func fileTransferServicesRetrieveFolderListingComplete(OBEXFileTransferServices!, error: OBEXError, listing: [Any]!)

func fileTransferServicesSendFileComplete(OBEXFileTransferServices!, error: OBEXError)

func fileTransferServicesSendFileProgress(OBEXFileTransferServices!, transferProgress: [AnyHashable : Any]!)

func handle(NSEvent!, client: Any!) -> Bool

Handles key down and mouse events.

func imageBrowser(IKImageBrowserView!, backgroundWasRightClickedWith: NSEvent!)

Performs custom tasks when the user right-clicks the image browser view background.

func imageBrowser(IKImageBrowserView!, cellWasDoubleClickedAt: Int)

Performs custom tasks when the user double-clicks an item in the image browser view.

func imageBrowser(IKImageBrowserView!, cellWasRightClickedAt: Int, with: NSEvent!)

Performs custom tasks when the user right-clicks an item in the image browser view.

func imageBrowser(IKImageBrowserView!, groupAt: Int) -> [AnyHashable : Any]!

Returns the group at the specified index.

func imageBrowser(IKImageBrowserView!, itemAt: Int) -> Any!

Returns an object for the item in an image browser view that corresponds to the specified index.

func imageBrowser(IKImageBrowserView!, moveItemsAt: IndexSet!, to: Int) -> Bool

Signals that the specified items should be moved to the specified destination.

func imageBrowser(IKImageBrowserView!, removeItemsAt: IndexSet!)

Signals that a remove operation should be applied to the specified items.

func imageBrowser(IKImageBrowserView!, writeItemsAt: IndexSet!, to: NSPasteboard!) -> Int

Signals that a drag should begin.

func imageBrowserSelectionDidChange(IKImageBrowserView!)

Performs custom tasks when the selection changes.

func imageRepresentation() -> Any!

Returns the image to display.

func imageRepresentationType() -> String!

Returns the representation type of the image to display.

func imageSubtitle() -> String!

Returns the display subtitle of the image.

func imageTitle() -> String!

Returns the display title of the image.

func imageUID() -> String!

Returns a unique string that identifies the data source item.

func imageVersion() -> Int

Returns the version of the item.

func index(ofAccessibilityElement: Any) -> Int

func indicesOfObjects(byEvaluatingObjectSpecifier: NSScriptObjectSpecifier) -> [NSNumber]?

Returns the indices of the specified container objects.

func inputText(String!, client: Any!) -> Bool

Handles key down events that do not map to an action method.

func inputText(String!, key: Int, modifiers: Int, client: Any!) -> Bool

Receives Unicode, the key code that generated it, and any modifier flags.

func isCaseInsensitiveLike(String) -> Bool

Returns a Boolean value that indicates whether receiver is considered to be “like” a given string when the case of characters in the receiver is ignored.

func isEqual(to: Any?) -> Bool

Returns a Boolean value that indicates whether the receiver is equal to another given object.

func isGreaterThan(Any?) -> Bool

Returns a Boolean value that indicates whether the receiver is greater than another given object.

func isGreaterThanOrEqual(to: Any?) -> Bool

Returns a Boolean value that indicates whether the receiver is greater than or equal to another given object.

func isLessThan(Any?) -> Bool

Returns a Boolean value that indicates whether the receiver is less than another given object.

func isLessThanOrEqual(to: Any?) -> Bool

Returns a Boolean value that indicates whether the receiver is less than or equal to another given object.

func isLike(String) -> Bool

Returns a Boolean value that indicates whether the receiver is “like” another given object.

func isNotEqual(to: Any?) -> Bool

Returns a Boolean value that indicates whether the receiver is not equal to another given object.

func numberOfGroups(inImageBrowser: IKImageBrowserView!) -> Int

Returns the number of groups in an image browser view.

func numberOfItems(inImageBrowser: IKImageBrowserView!) -> Int

Returns the number of records managed by the data source object.

func originalString(Any!) -> NSAttributedString!

Return the string that consists of the precomposed Unicode characters.

func performAction(for: ABPerson!, identifier: String!)

Sent to the delegate to perform the action.

func prepareForInterfaceBuilder()

Called when a designable object is created in Interface Builder.

func provideImageData(UnsafeMutableRawPointer, bytesPerRow: Int, origin: Int, Int, size: Int, Int, userInfo: Any?)

Supplies data to a `CIImage` object.

func quartzFilterManager(QuartzFilterManager!, didAdd: QuartzFilter!)

func quartzFilterManager(QuartzFilterManager!, didModifyFilter: QuartzFilter!)

func quartzFilterManager(QuartzFilterManager!, didRemove: QuartzFilter!)

func quartzFilterManager(QuartzFilterManager!, didSelect: QuartzFilter!)

func readLinkQuality(forDeviceComplete: Any!, device: IOBluetoothDevice!, info: UnsafeMutablePointer&lt;BluetoothHCILinkQualityInfo>!, error: IOReturn)

func readRSSI(forDeviceComplete: Any!, device: IOBluetoothDevice!, info: UnsafeMutablePointer&lt;BluetoothHCIRSSIInfo>!, error: IOReturn)

func saveOptions(IKSaveOptions!, shouldShowUTType: String!) -> Bool

Called to determine if the specified uniform type identifier should be shown in the save panel.

func setSharedObservers(NSKeyValueSharedObserversSnapshot?)

func setupPanel(DRSetupPanel!, determineBestDeviceOfA: DRDevice!, orB: DRDevice!) -> DRDevice!

Allows the delegate to specify which device is its preferred.

func setupPanel(DRSetupPanel!, deviceContainsSuitableMedia: DRDevice!, promptString: AutoreleasingUnsafeMutablePointer&lt;NSString?>!) -> Bool

This delegate method allows the delegate to determine if the media inserted in the device is suitable for whatever operation is to be performed.

func setupPanel(DRSetupPanel!, deviceCouldBeTarget: DRDevice!) -> Bool

Allows the delegate to determine if device can be used as a target.

func setupPanelDeviceSelectionChanged(Notification!)

Sent by the default notification center when the device selection in the panel has changed.

func setupPanelShouldHandleMediaReservations(DRSetupPanel!) -> Bool

This delegate method allows the delegate to control how media reservations are handled.

func shouldEnableAction(for: ABPerson!, identifier: String!) -> Bool

Sent to the delegate to determine whether the action should be enabled.

func title(for: ABPerson!, identifier: String!) -> String!

Sent to the delegate to request the title of the menu item for the action.

func workflowController(AMWorkflowController, didError: any Error)Deprecated

func workflowController(AMWorkflowController, didRun: AMAction)Deprecated

func workflowController(AMWorkflowController, willRun: AMAction)Deprecated

func workflowControllerDidRun(AMWorkflowController)Deprecated

func workflowControllerDidStop(AMWorkflowController)Deprecated

func workflowControllerWillRun(AMWorkflowController)Deprecated

func workflowControllerWillStop(AMWorkflowController)Deprecated

### Type Methods

class func debugDescription() -> String

class func hash() -> Int

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Classes

class Protocol

