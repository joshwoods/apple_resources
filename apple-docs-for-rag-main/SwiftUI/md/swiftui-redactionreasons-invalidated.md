

- SwiftUI
- RedactionReasons
-  invalidated 

Type Property

# invalidated

Displayed data should appear as invalidated and pending a new update.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let invalidated: RedactionReasons
```

## Discussion

Views marked with `invalidatableContent` will be automatically redacted with a standard styling indicating the content is invalidated and new content will be available soon.

## See Also

### Getting redaction reasons

static let placeholder: RedactionReasons

Displayed data should appear as generic placeholders.

static let privacy: RedactionReasons

Displayed data should be obscured to protect private information.

