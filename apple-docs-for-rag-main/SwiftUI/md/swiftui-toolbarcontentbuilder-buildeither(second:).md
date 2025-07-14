

- SwiftUI
- ToolbarContentBuilder
-  buildEither(second:) 

Type Method

# buildEither(second:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func buildEither(second: FalseContent) -> _ConditionalContent where TrueContent : CustomizableToolbarContent, FalseContent : CustomizableToolbarContent
```

Show all declarations

## See Also

### Building conditional toolbar content

static buildIf(_:)

static buildEither(first:)

static buildExpression(_:)

Builds an expression within the builder.

static buildLimitedAvailability(_:)

