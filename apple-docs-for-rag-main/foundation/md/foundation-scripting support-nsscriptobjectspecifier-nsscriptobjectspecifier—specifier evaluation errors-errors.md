

- Foundation
- Scripting Support
- NSScriptObjectSpecifier
-  NSScriptObjectSpecifier—Specifier Evaluation Errors 

API Collection

# NSScriptObjectSpecifier—Specifier Evaluation Errors

`NSScriptObjectSpecifier` provides the following constants for error codes for specific problems evaluating specifiers:

## Topics

### Constants

var NSNoSpecifierError: Int

No error encountered.

var NSNoTopLevelContainersSpecifierError: Int

Someone called `evaluate` with `nil`.

var NSContainerSpecifierError: Int

Error evaluating container specifier.

var NSUnknownKeySpecifierError: Int

Receivers do not understand the key.

var NSInvalidIndexSpecifierError: Int

Index out of bounds.

var NSInternalSpecifierError: Int

Other internal error.

var NSOperationNotSupportedForKeySpecifierError: Int

Attempt made to perform an unsupported operation on some key.

