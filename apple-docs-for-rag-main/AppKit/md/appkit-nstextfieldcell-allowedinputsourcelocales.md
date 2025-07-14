

- AppKit
- NSTextFieldCell
-  allowedInputSourceLocales 

Instance Property

# allowedInputSourceLocales

An array of locale identifiers that represent the allowed input sources when the text field has the keyboard focus.

macOS 10.5+

``` source
@MainActor
var allowedInputSourceLocales: [String]? { get set }
```

## Discussion

The value of this property is an array of NSString objects, each of which contains a locale identifier. You can assign the meta-locale identifier, NSAllRomanInputSourcesLocaleIdentifier, to specify input sources that are limited for Roman script editing.

