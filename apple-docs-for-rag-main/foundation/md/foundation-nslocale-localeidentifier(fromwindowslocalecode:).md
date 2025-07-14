

- Foundation
- NSLocale
-  localeIdentifier(fromWindowsLocaleCode:) 

Type Method

# localeIdentifier(fromWindowsLocaleCode:)

Returns a locale identifier from a Windows locale code.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func localeIdentifier(fromWindowsLocaleCode lcid: UInt32) -> String?
```

## Parameters 

`lcid`  

The Windows locale code.

## Return Value

The locale identifier.

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

class func windowsLocaleCode(fromLocaleIdentifier: String) -> UInt32

Returns a Window locale code from the locale identifier.

