

- GLKit
- GLKTextureLoader
-  Texture Error Handling 

API Collection

# Texture Error Handling

Strings used when handling error messages returned from a texture loading method.

## Topics

### Constants

let GLKTextureLoaderErrorDomain: String

The error domain used by GLKit when returning texture loading errors.

Deprecated

let GLKTextureLoaderErrorKey: String

A key used to retrieve an error string from an error object userinfo dictionary.

Deprecated

let GLKTextureLoaderGLErrorKey: String

A key used to retrieve additional information from an error object’s userinfo dictionary.

Deprecated

## See Also

### Constants

typealias GLKTextureLoaderCallback

Signature for the block executed after an asynchronous texture loading operation completes.

Texture Loading Options

Keys to specify in a `textureOperations` dictionary.

enum Code

Values to be returned when a texture loader encounters an error.

