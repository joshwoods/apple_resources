

- Core Text
-  kCTTypesetterOptionDisableBidiProcessing Deprecated

Global Variable

# kCTTypesetterOptionDisableBidiProcessing

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
let kCTTypesetterOptionDisableBidiProcessing: CFString
```

Deprecated

Deprecated

## Discussion

Disables bidirectional processing. Value must be a CFBoolean object. Default value is `false`. Normally, typesetting applies the Unicode Bidirectional Algorithm as described in Unicode Standard Annex \#9. If a typesetter is created with this option set to `true`, no directional reordering is performed, and any directional control characters are ignored.

## See Also

### Constants

let kCTTypesetterOptionForcedEmbeddingLevel: CFString

A key that specifies the embedding level of the typesetter’s text.

let kCTTypesetterOptionAllowUnboundedLayout: CFString

A key that specifies whether the text system lays out text that requires unreasonable effort.

