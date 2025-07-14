

- SwiftUI
- CommandsBuilder
-  buildBlock(\_:\_:\_:\_:\_:\_:\_:\_:) 

Type Method

# buildBlock(\_:\_:\_:\_:\_:\_:\_:\_:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
static func buildBlock(
    _ c0: C0,
    _ c1: C1,
    _ c2: C2,
    _ c3: C3,
    _ c4: C4,
    _ c5: C5,
    _ c6: C6,
    _ c7: C7
) -> some Commands where C0 : Commands, C1 : Commands, C2 : Commands, C3 : Commands, C4 : Commands, C5 : Commands, C6 : Commands, C7 : Commands
```

## See Also

### Building content

static func buildBlock() -> EmptyCommands

Builds an empty command set from a block containing no statements.

static func buildBlock&lt;C>(C) -> C

Passes a single command group written as a child group through modified.

static func buildBlock&lt;C0, C1>(C0, C1) -> some Commands

static func buildBlock&lt;C0, C1, C2>(C0, C1, C2) -> some Commands

static func buildBlock&lt;C0, C1, C2, C3>(C0, C1, C2, C3) -> some Commands

static func buildBlock&lt;C0, C1, C2, C3, C4>(C0, C1, C2, C3, C4) -> some Commands

static func buildBlock&lt;C0, C1, C2, C3, C4, C5>(C0, C1, C2, C3, C4, C5) -> some Commands

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6>(C0, C1, C2, C3, C4, C5, C6) -> some Commands

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8>(C0, C1, C2, C3, C4, C5, C6, C7, C8) -> some Commands

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9) -> some Commands

