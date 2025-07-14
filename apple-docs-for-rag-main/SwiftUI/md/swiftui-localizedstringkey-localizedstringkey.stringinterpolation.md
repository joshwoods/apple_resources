

- SwiftUI
- LocalizedStringKey
-  LocalizedStringKey.StringInterpolation 

Structure

# LocalizedStringKey.StringInterpolation

Represents the contents of a string literal with interpolations while it’s being built, for use in creating a localized string key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct StringInterpolation
```

## Topics

### Appending to an interpolation

The compiler uses these methods when interpreting string interpolations; don’t call them directly.

func appendInterpolation(_:)

Appends an attributed string to a string interpolation.

func appendInterpolation&lt;T>(T, specifier: String)

Appends a type, convertible to a string with a format specifier, to a string interpolation.

func appendInterpolation(_:format:)

Appends the formatted representation of a nonstring type supported by a corresponding format style.

func appendInterpolation(_:formatter:)

Appends an optionally-formatted instance of an Objective-C subclass to a string interpolation.

func appendInterpolation(Date, style: Text.DateStyle)

Appends a formatted date to a string interpolation.

func appendInterpolation(timerInterval: ClosedRange&lt;Date>, pauseTime: Date?, countsDown: Bool, showsHours: Bool)

Appends a timer interval to a string interpolation.

func appendLiteral(String)

Appends a literal string.

### Instance Methods

func appendInterpolation(accessibilityName: Color)

Appends a localized description of a color for accessibility to a string interpolation.

## Relationships

### Conforms To

- StringInterpolationProtocol

## See Also

### Creating a key from an interpolation

init(stringInterpolation: LocalizedStringKey.StringInterpolation)

Creates a localized string key from the given string interpolation.

