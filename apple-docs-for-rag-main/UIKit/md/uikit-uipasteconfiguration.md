

- UIKit
-  UIPasteConfiguration 

Class

# UIPasteConfiguration

The interface that an object implements to declare its ability to accept specific data types for pasting and for drag-and-drop activities.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIPasteConfiguration
```

## Topics

### Initializing a paste configuration

init()

Initializes a new paste configuration.

convenience init(acceptableTypeIdentifiers: [String])

Initializes a new paste configuration with a specified array of acceptable UTIs.

convenience init(forAccepting: any NSItemProviderReading.Type)

Initializes a new paste configuration with the UTIs declared as supported by a specified class.

convenience init&lt;T>(forAccepting: T.Type)

### Getting acceptable type identifiers

var acceptableTypeIdentifiers: [String]

An array of UTI strings that specify the types accepted by the paste configuration.

### Adding acceptable type identifiers

func addAcceptableTypeIdentifiers([String])

Adds an array of UTI strings to a paste configuration, increasing the variety of types the paste configuration accepts.

func addTypeIdentifiers(forAccepting: any NSItemProviderReading.Type)

Expands the array of accepted UTIs for a paste configuration, based on those declared as supported by a specified class.

func addTypeIdentifiers&lt;T>(forAccepting: T.Type)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Pasteboard

class UIPasteControl

A button that a person taps to place pasteboard contents in your app.

class Configuration

An object that determines a paste button’s color, corner style, icon, and text.

enum DisplayMode

Options that determine whether a paste button composes an icon, textual label, or both.

class UIPasteboard

An object that helps a user share data from one place to another within your app, and from your app to other apps.

protocol UIPasteConfigurationSupporting

The interface that determines whether a responder object supports paste configuration.

