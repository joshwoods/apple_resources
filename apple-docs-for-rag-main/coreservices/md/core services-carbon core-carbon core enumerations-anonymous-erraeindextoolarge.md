

- Core Services
- Carbon Core
- Carbon Core Enumerations
- Anonymous
-  errAEIndexTooLarge 

Global Variable

# errAEIndexTooLarge

The index of the event is too large to bevalid.

Mac Catalyst 13.0+macOS 10.0+

``` source
var errAEIndexTooLarge: Int { get }
```

## See Also

### Result Codes

var noPortErr: Int

Client hasn’t set `'SIZE'` resource toindicate awareness of high-level events

var destPortErr: Int

Server hasn’t set `'SIZE'` resource toindicate awareness of high-level events, or else is not present

var sessClosedErr: Int

The `kAEDontReconnect` flagin the `sendMode` parameterwas set and the server quit, then restarted

var errAECoercionFail: Int

Data could not be coerced to the requesteddescriptor type

var errAEDescNotFound: Int

Descriptor was not found

var errAECorruptData: Int

Data in an Apple event could not be read

var errAEWrongDataType: Int

Wrong descriptor type

var errAENotAEDesc: Int

Not a valid descriptor

var errAEBadListItem: Int

Operation involving a list item failed

var errAENewerVersion: Int

Need a newer version of the Apple EventManager

var errAENotAppleEvent: Int

The event is not in AppleEvent format.

var errAEEventNotHandled: Int

Event wasn’t handled by an Apple eventhandler

var errAEReplyNotValid: Int

`AEResetTimer` was passed an invalid reply

var errAEUnknownSendMode: Int

Invalid sending mode was passed

var errAEWaitCanceled: Int

User canceled out of wait loop for replyor receipt

var errAETimeout: Int

Apple event timed out

var errAENoUserInteraction: Int

No user interaction allowed

var errAENotASpecialFunction: Int

Wrong keyword for a special function

var errAEParamMissed: Int

A required parameter was not accessed.

var errAEUnknownAddressType: Int

Unknown Apple event address type

var errAEHandlerNotFound: Int

No handler found for an Apple event

var errAEReplyNotArrived: Int

Reply has not yet arrived

var errAEIllegalIndex: Int

Not a valid list index

var errAEImpossibleRange: Int

The range is not valid because it is impossiblefor a range to include the first and last objects that were specified;an example is a range in which the offset of the first object is greaterthan the offset of the last object

var errAEWrongNumberArgs: Int

The number of operands provided for the `kAENOT` logicaloperator is not 1

var errAEAccessorNotFound: Int

There is no object accessor function forthe specified object class and container type

var errAENoSuchLogical: Int

The logical operator in a logical descriptoris not `kAEAND`, `kAEOR`,or `kAENOT`

var errAEBadTestKey: Int

The descriptor in a test key is neithera comparison descriptor nor a logical descriptor

var errAENoSuchObject: Int

Runtime resolution of an object failed.

var errAENegativeCount: Int

An object-counting function returned a negativeresult

var errAEEmptyListContainer: Int

The container for an Apple event objectis specified by an empty list

var errAEUnknownObjectType: Int

The object type isn’t recognized

var errAERecordingIsAlreadyOn: Int

Recording is already on

var errAEReceiveTerminate: Int

Break out of all levels of `AEReceive` tothe topmost (1.1 or greater)

var errAEReceiveEscapeCurrent: Int

Break out of lowest level only of `AEReceive` (1.1or greater)

var errAEEventFiltered: Int

Event has been filtered and should not bepropagated (1.1 or greater)

var errAEDuplicateHandler: Int

Attempt to install handler in table foridentical class and ID (1.1 or greater)

var errAEStreamBadNesting: Int

Nesting violation while streaming

var errAEStreamAlreadyConverted: Int

Attempt to convert a stream that has alreadybeen converted

var errAEDescIsNull: Int

Attempt to perform an invalid operationon a null descriptor

var errAEBuildSyntaxError: Int

`AEBuildDesc` andrelated functions detected a syntax error

var errAEBufferTooSmall: Int

Buffer for `AEFlattenDesc` toosmall

var errASCantConsiderAndIgnore: Int

Can’t both consider and ignore \.

var errASCantCompareMoreThan32k: Int

Can’t perform operation on text longerthan 32K bytes.

var errASTerminologyNestingTooDeep: Int

Tell statements are nested too deeply.

var errASIllegalFormalParameter: Int

\ is illegal as a formal parameter.

var errASParameterNotForEvent: Int

\ is not a parameter name for the event \.

var errASNoResultReturned: Int

No result was returned for some argumentof this expression.

var errAEEventFailed: Int

Apple event handler failed.

var errAETypeError: Int

A descriptor type mismatch occurred.

var errAEBadKeyForm: Int

Invalid key form.

var errAENotModifiable: Int

Can't set \ to \. Access not allowed.

var errAEPrivilegeError: Int

A privilege violation occurred.

var errAEReadDenied: Int

The read operation was not allowed.

var errAEWriteDenied: Int

Can't set \ to \.

var errAENotAnElement: Int

The specified object is a property, notan element.

var errAECantSupplyType: Int

Can’t supply the requested descriptortype for the data.

var errAECantHandleClass: Int

The Apple event handler can’t handle objectsof this class.

var errAEInTransaction: Int

Couldn’t handle this command because itwasn’t part of the current transaction.

var errAENoSuchTransaction: Int

The transaction to which this command belongedisn’t a valid transaction.

var errAENoUserSelection: Int

There is no user selection.

var errAENotASingleObject: Int

Handler only handles single objects.

var errAECantUndo: Int

Can’t undo the previous Apple event oruser action.

var errAENotAnEnumMember: Int

Enumerated value in `SetData` is notallowed for this property

var errAECantPutThatThere: Int

In make new, duplicate, etc. class can'tbe an element of container

var errAEPropertiesClash: Int

Illegal combination of properties settingsfor SetData, make new, or duplicate

