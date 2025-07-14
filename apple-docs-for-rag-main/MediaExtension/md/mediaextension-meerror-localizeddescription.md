

- MediaExtension
- MEError
-  localizedDescription 

Instance Property

# localizedDescription

A string that contains the localized description of the error.

MediaExtensionSwiftiOS 8.0+iPadOS 8.0+macOS 10.10+tvOS 9.0+watchOS 2.0+

``` source
var localizedDescription: String { get }
```

## See Also

### Inspecting an error

var code: Int

The error code.

var errorCode: Int

var errorUserInfo: [String : Any]

var hashValue: Int { get }

The hash value.

var userInfo: [String : Any]

The user info dictionary.

static func == (lhs: Self, rhs: Self) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (lhs: Self, rhs: Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into hasher: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

enum Code

An enumeration that models media extension error codes.

