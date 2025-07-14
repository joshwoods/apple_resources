

- SwiftUI
- Font
-  init(\_:) 

Initializer

# init(\_:)

Creates a custom font from a platform font instance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ font: CTFont)
```

## Discussion

Initializing Font with platform font instance (doc://com.apple.documentation/documentation/CoreText/CTFont-q6r) can bridge SwiftUI Font with NSFont or UIFont, both of which are toll-free bridged to doc://com.apple.documentation/documentation/CoreText/CTFont-q6r. For example:

```
// Use native Core Text API to create desired ctFont.
let ctFont = CTFontCreateUIFontForLanguage(.system, 12, nil)!

// Create SwiftUI Text with the CTFont instance.
let text = Text("Hello").font(Font(ctFont))
```

