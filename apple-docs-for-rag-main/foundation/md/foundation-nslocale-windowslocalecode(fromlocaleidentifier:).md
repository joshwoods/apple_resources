

- Foundation
- NSLocale
-  windowsLocaleCode(fromLocaleIdentifier:) 

Type Method

# windowsLocaleCode(fromLocaleIdentifier:)

Returns a Window locale code from the locale identifier.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func windowsLocaleCode(fromLocaleIdentifier localeIdentifier: String) -> UInt32
```

## Parameters 

`localeIdentifier`  

The locale identifier.

## Return Value

The Windows locale code.

## See Also

### Converting Between Identifiers

class func canonicalLocaleIdentifier(from: String) -> String

Returns the canonical identifier for a given locale identification string.

class func components(fromLocaleIdentifier: String) -> [String : String]

Returns a dictionary that is the result of parsing a locale ID.

class func localeIdentifier(fromComponents: [String : String]) -> String

Returns a locale identifier from the components specified in a given dictionary.

class func canonicalLanguageIdentifier(from: String) -> String

Returns a canonical language identifier by mapping an arbitrary locale identification string to the canonical identifier.

class func localeIdentifier(fromWindowsLocaleCode: UInt32) -> String?

Returns a locale identifier from a Windows locale code.

