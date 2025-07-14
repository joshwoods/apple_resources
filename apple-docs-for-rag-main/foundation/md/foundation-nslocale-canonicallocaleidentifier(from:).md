

- Foundation
- NSLocale
-  canonicalLocaleIdentifier(from:) 

Type Method

# canonicalLocaleIdentifier(from:)

Returns the canonical identifier for a given locale identification string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func canonicalLocaleIdentifier(from string: String) -> String
```

## Parameters 

`string`  

A locale identification string.

## Return Value

The canonical identifier for an the locale identified by `string`.

## See Also

### Converting Between Identifiers

class func components(fromLocaleIdentifier: String) -> [String : String]

Returns a dictionary that is the result of parsing a locale ID.

class func localeIdentifier(fromComponents: [String : String]) -> String

Returns a locale identifier from the components specified in a given dictionary.

class func canonicalLanguageIdentifier(from: String) -> String

Returns a canonical language identifier by mapping an arbitrary locale identification string to the canonical identifier.

class func localeIdentifier(fromWindowsLocaleCode: UInt32) -> String?

Returns a locale identifier from a Windows locale code.

class func windowsLocaleCode(fromLocaleIdentifier: String) -> UInt32

Returns a Window locale code from the locale identifier.

