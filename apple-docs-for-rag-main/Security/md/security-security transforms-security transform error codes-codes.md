

- Security
- Security Transforms
-  Security Transform Error Codes 

API Collection

# Security Transform Error Codes

Recognize the error codes used in error objects created by a transform on failure.

## Topics

### Constants

var kSecTransformErrorAttributeNotFound: CFIndex

The attribute was not found.

var kSecTransformErrorInvalidOperation: CFIndex

An invalid operation was attempted.

var kSecTransformErrorNotInitializedCorrectly: CFIndex

A required initialization is missing: It is most likely a missing required attribute.

var kSecTransformErrorMoreThanOneOutput: CFIndex

A transform has an internal routing error that has caused multiple outputs instead of a single discrete output.

var kSecTransformErrorInvalidInputDictionary: CFIndex

A dictionary used to import a transform has invalid data.

var kSecTransformErrorInvalidAlgorithm: CFIndex

A transform that needs an algorithm as an attribute received an invalid algorithm.

var kSecTransformErrorInvalidLength: CFIndex

A transform that needs a length such as a digest transform has been given an invalid length.

var kSecTransformErrorInvalidType: CFIndex

An invalid type has been set on an attribute.

var kSecTransformErrorInvalidInput: CFIndex

The input set on a transform is invalid.

var kSecTransformErrorNameAlreadyRegistered: CFIndex

A custom transform of a particular name has already been registered.

var kSecTransformErrorUnsupportedAttribute: CFIndex

An illegal action such as setting a read-only attribute has occurred.

var kSecTransformOperationNotSupportedOnGroup: CFIndex

An illegal action on a group transform has occurred.

var kSecTransformErrorMissingParameter: CFIndex

A transform is missing a required attribute.

var kSecTransformErrorInvalidConnection: CFIndex

A connection between transforms in different groups was attempted.

var kSecTransformTransformIsExecuting: CFIndex

An illegal operation was called on a Transform while it was executing.

var kSecTransformInvalidOverride: CFIndex

An illegal override was given to a custom transform.

var kSecTransformTransformIsNotRegistered: CFIndex

A custom transform was asked to be created but the transform has not been registered.

var kSecTransformErrorAbortInProgress: CFIndex

The abort attribute has been set and the transform is in the process of shutting down.

var kSecTransformErrorAborted: CFIndex

The transform was aborted.

var kSecTransformInvalidArgument: CFIndex

An invalid argument was given to a Transform API.

