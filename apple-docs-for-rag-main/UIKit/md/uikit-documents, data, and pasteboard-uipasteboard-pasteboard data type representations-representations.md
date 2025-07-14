

- UIKit
- Documents, data, and pasteboard
- UIPasteboard
-  Pasteboard Data Type Representations 

API Collection

# Pasteboard Data Type Representations

Pasteboard-item representation types, as for a given object value.

## Topics

### Constants

class var typeListString: NSArray

An array of pasteboard-item representation types for string-type uniform type identifiers (UTIs), including the `kUTTypeUTF8PlainText` and `kUTTypeText` types. Related UIPasteboard properties are string and strings.

class var typeListURL: NSArray

An array of pasteboard-item representation types for URL-type uniform type identifiers (UTIs), including `kUTTypeURL`. Related UIPasteboard properties are url and urls.

class var typeListImage: NSArray

An array of pasteboard-item representation types for image-type uniform type identifiers (UTIs), including `kUTTypePNG` and `kUTTypeJPEG`. Related UIPasteboard properties are image and images.

class var typeListColor: NSArray

An array of pasteboard-item representation types for colors. Related UIPasteboard properties are color and colors.

class let typeAutomatic: String

An array of pasteboard-item representation types with automatically-determined uniform type identifiers (UTIs).

## See Also

### Constants

struct Name

Constants that identify the name of a pasteboard.

Pasteboard Names

Names identifying the system pasteboards.

struct OptionsKey

Options for describing pasteboard privacy.

UserInfo Dictionary Keys

Use these keys to access the representation types of pasteboard items that you add to, or remove from, a pasteboard.

