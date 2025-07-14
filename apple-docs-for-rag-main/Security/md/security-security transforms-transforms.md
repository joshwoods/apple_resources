

- Security
-  Security Transforms 

API Collection

# Security Transforms

Perform cryptographic functions like encoding, encryption, signing, and signature verification.

## Overview

You use security transforms to assemble a chain of security-related operations that you apply to a stream of data in macOS.

## Topics

### Transforms

func SecTransformCreateReadTransformWithReadStream(CFReadStream) -> SecTransform

Creates a read transform from a read stream reference.

Deprecated

typealias SecTransform

A Core Foundation type that represents a security transform.

Deprecated

func SecTransformGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which a security transform object belongs.

Deprecated

### Encoding

func SecEncodeTransformCreate(CFTypeRef, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecTransform?

Creates an encode transform object.

Deprecated

func SecDecodeTransformCreate(CFTypeRef, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecTransform?

Creates a decode transform object.

Deprecated

### Encrypting

func SecEncryptTransformCreate(SecKey, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecTransform

Creates an encryption transform object.

Deprecated

func SecDecryptTransformCreate(SecKey, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecTransform

Creates a decryption transform object.

Deprecated

func SecEncryptTransformGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which an encryption transform belongs.

Deprecated

func SecDecryptTransformGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which a decryption transform belongs.

Deprecated

### Signing

func SecSignTransformCreate(SecKey, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecTransform?

Creates a signing transform object.

Deprecated

func SecVerifyTransformCreate(SecKey, CFData?, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecTransform?

Creates a verify transform object.

Deprecated

func SecDigestTransformCreate(CFTypeRef?, CFIndex, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecTransform

Creates a digest transform object.

Deprecated

func SecDigestTransformGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which a digest transform belongs.

Deprecated

### Custom Transforms

func SecTransformCreate(CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecTransform?

Creates a transform computation object.

Deprecated

func SecTransformRegister(CFString, SecTransformCreateFP, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

Registers a custom transform.

Deprecated

typealias SecTransformCreateFP

A pointer to a function that creates a new instance of a custom transform.

Deprecated

typealias SecTransformInstanceBlock

A block that you return from a transform creation function.

typealias SecTransformImplementationRef

An opaque pointer to a block that implements an instance of a transform.

### Transform Groups

func SecTransformCreateGroupTransform() -> SecGroupTransform

Creates an object that acts as a container for a set of connected transforms.

Deprecated

func SecTransformFindByName(SecGroupTransform, CFString) -> SecTransform?

Finds a member of a transform group by its name.

Deprecated

typealias SecGroupTransform

A Core Foundation type that represents a container holding a group of transforms.

Deprecated

func SecGroupTransformGetTypeID() -> CFTypeID

Returns the Core Foundation type ID for a transform group container.

Deprecated

### Transform Characteristics

func SecTransformSetAttribute(SecTransform, CFString, CFTypeRef, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Bool

Sets a static value for an attribute in a transform.

Deprecated

func SecTransformGetAttribute(SecTransform, CFString) -> CFTypeRef?

Gets the current value of a transform attribute.

Deprecated

func SecTransformCustomSetAttribute(SecTransformImplementationRef, SecTransformStringOrAttribute, SecTransformMetaAttributeType, CFTypeRef?) -> CFTypeRef?

Sets an attribute value on a custom transform.

Deprecated

func SecTransformCustomGetAttribute(SecTransformImplementationRef, SecTransformStringOrAttribute, SecTransformMetaAttributeType) -> CFTypeRef?

Gets an attribute value from a custom transform.

Deprecated

func SecTransformPushbackAttribute(SecTransformImplementationRef, SecTransformStringOrAttribute, CFTypeRef) -> CFTypeRef?

Pushes a single value back for a specific attribute.

Deprecated

Transform Attributes

Specify the attributes of a transform.

typealias SecTransformAttribute

A direct reference to a security transform attribute.

Deprecated

typealias SecTransformStringOrAttribute

A type that may be either a string or an attribute reference.

Deprecated

enum SecTransformMetaAttributeType

The keys that describe the metadata attributes of transform attributes.

Deprecated

### Actions

func SecTransformSetDataAction(SecTransformImplementationRef, CFString, SecTransformDataBlock) -> CFError?

Changes the way a custom transform processes data.

Deprecated

func SecTransformSetAttributeAction(SecTransformImplementationRef, CFString, SecTransformStringOrAttribute?, SecTransformAttributeActionBlock) -> CFError?

Requests a callback when an attribute is set.

Deprecated

func SecTransformSetTransformAction(SecTransformImplementationRef, CFString, SecTransformActionBlock) -> CFError?

Changes the way that a transform deals with transform lifecycle behaviors.

Deprecated

typealias SecTransformActionBlock

A block that overrides the default behavior of a custom transform.

Deprecated

typealias SecTransformAttributeActionBlock

A block used to override the default attribute handling for when an attribute is set.

Deprecated

typealias SecTransformDataBlock

A block used to override the default data handling for a transform.

Actions

Use actions to trigger particular behaviors.

### Piping

func SecTransformConnectTransforms(SecTransform, CFString, SecTransform, CFString, SecGroupTransform, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecGroupTransform?

Chains transforms together.

Deprecated

### Execution

func SecTransformExecute(SecTransform, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> CFTypeRef

Executes a transform or transform group synchronously.

Deprecated

func SecTransformExecuteAsync(SecTransform, dispatch_queue_t, SecMessageBlock)

Executes transform or transform group asynchronously.

Deprecated

func SecTransformNoData() -> CFTypeRef

Returns an object from inside a ProcessData override that says that although no data is being returned the transform is still active and awaiting data.

Deprecated

typealias SecMessageBlock

A block that delivers messages during asynchronous operations.

### Import and Export

func SecTransformCopyExternalRepresentation(SecTransform) -> CFDictionary

Creates a dictionary that contains enough information to be able to recreate a transform.

Deprecated

func SecTransformCreateFromExternalRepresentation(CFDictionary, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> SecTransform?

Creates a transform instance from a dictionary of parameters.

Deprecated

### Reporting Errors

let kSecTransformErrorDomain: CFString

The domain of any error object created by a transform on failure.

Security Transform Error Codes

Recognize the error codes used in error objects created by a transform on failure.

let kSecTransformPreviousErrorKey: CFString

The key in an error’s `userInfo` dictionary whose value specifies the previous error when multiple errors occur during transform evaluation.

let kSecTransformAbortOriginatorKey: CFString

The key in an error’s `userInfo` dictionary whose value indicates the transform that caused the chain to abort.

## See Also

### Related Documentation

Security Transforms Programming Guide

