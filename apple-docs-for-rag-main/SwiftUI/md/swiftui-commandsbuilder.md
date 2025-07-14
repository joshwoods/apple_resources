

- SwiftUI
-  CommandsBuilder 

Structure

# CommandsBuilder

Constructs command sets from multi-expression closures. Like `ViewBuilder`, it supports up to ten expressions in the closure body.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@resultBuilder
struct CommandsBuilder
```

## Topics

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

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7>(C0, C1, C2, C3, C4, C5, C6, C7) -> some Commands

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8>(C0, C1, C2, C3, C4, C5, C6, C7, C8) -> some Commands

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9) -> some Commands

### Building conditionally

static func buildEither&lt;T, F>(first: T) -> _ConditionalContent&lt;T, F>

Produces content for a conditional statement in a multi-statement closure when the condition is true.

static func buildEither&lt;T, F>(second: F) -> _ConditionalContent&lt;T, F>

Produces content for a conditional statement in a multi-statement closure when the condition is false.

static func buildIf&lt;C>(C?) -> C?

Produces an optional widget for conditional statements in multi-statement closures that’s only visible when the condition evaluates to true.

static buildLimitedAvailability(_:)

Processes commands for a conditional compiler-control statement that performs an availability check.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

## See Also

### Defining commands

func commands&lt;Content>(content: () -> Content) -> some Scene

Adds commands to the scene.

func commandsRemoved() -> some Scene

Removes all commands defined by the modified scene.

func commandsReplaced&lt;Content>(content: () -> Content) -> some Scene

Replaces all commands defined by the modified scene with the commands from the builder.

protocol Commands

Conforming types represent a group of related commands that can be exposed to the user via the main menu on macOS and key commands on iOS.

struct CommandMenu

Command menus are stand-alone, top-level containers for controls that perform related, app-specific commands.

struct CommandGroup

Groups of controls that you can add to existing command menus.

struct CommandGroupPlacement

The standard locations that you can place new command groups relative to.

