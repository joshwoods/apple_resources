

- TipKit
- Tips
-  Tips.GroupBuilder 

Structure

# Tips.GroupBuilder

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@resultBuilder
struct GroupBuilder
```

## Topics

### Type Methods

static func buildArray([[any Tip]]) -> [any Tip]

static func buildBlock() -> [any Tip]

static func buildBlock(any Tip...) -> [any Tip]

static func buildEither(first: [any Tip]) -> [any Tip]

static func buildEither(second: [any Tip]) -> [any Tip]

static func buildIf([any Tip]?) -> [any Tip]

static func buildPartialBlock(accumulated: [any Tip], next: [any Tip]) -> [any Tip]

static func buildPartialBlock(accumulated: [any Tip], next: any Tip) -> [any Tip]

static func buildPartialBlock(first: [any Tip]) -> [any Tip]

static func buildPartialBlock(first: Never) -> [any Tip]

static func buildPartialBlock(first: any Tip) -> [any Tip]

static func buildPartialBlock(first: Void) -> [any Tip]

