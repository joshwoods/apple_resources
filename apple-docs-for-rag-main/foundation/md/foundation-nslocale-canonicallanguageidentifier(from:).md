

- Foundation
- NSLocale
-  canonicalLanguageIdentifier(from:) 

Type Method

# canonicalLanguageIdentifier(from:)

Returns a canonical language identifier by mapping an arbitrary locale identification string to the canonical identifier.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func canonicalLanguageIdentifier(from string: String) -> String
```

## Parameters 

`string`  

A string representation of an arbitrary locale identifier.

## Return Value

A string that represents the canonical language identifier for the specified arbitrary locale identifier.

## See Also

### Converting Between Identifiers

class func canonicalLocaleIdentifier(from: String) -> String

Returns the canonical identifier for a given locale identification string.

class func components(fromLocaleIdentifier: String) -> [String : String]

Returns a dictionary that is the result of parsing a locale ID.

class func localeIdentifier(fromComponents: [String : String]) -> String

Returns a locale identifier from the components specified in a given dictionary.

class func localeIdentifier(fromWindowsLocaleCode: UInt32) -> String?

Returns a locale identifier from a Windows locale code.

class func windowsLocaleCode(fromLocaleIdentifier: String) -> UInt32

Returns a Window locale code from the locale identifier.

