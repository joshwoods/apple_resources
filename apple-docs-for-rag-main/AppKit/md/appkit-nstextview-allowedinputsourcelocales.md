

- AppKit
- NSTextView
-  allowedInputSourceLocales 

Instance Property

# allowedInputSourceLocales

An array of locale identifiers representing input sources that are allowed to be enabled when the receiver has the keyboard focus.

macOS 10.5+

``` source
@MainActor
var allowedInputSourceLocales: [String]? { get set }
```

## Discussion

You can use the meta-locale identifier, NSAllRomanInputSourcesLocaleIdentifier, to specify input sources that are limited for Roman script editing.

## See Also

### Inserting text

func insertText(Any)

Inserts `aString` into the receiver’s text at the insertion point if there is one, otherwise replacing the selection.

Deprecated

