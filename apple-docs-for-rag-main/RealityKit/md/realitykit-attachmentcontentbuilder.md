

- RealityKit
-  AttachmentContentBuilder 

Structure

# AttachmentContentBuilder

A result builder that creates attachment content from closures.

RealityKitSwiftUIvisionOS 1.0+

``` source
@resultBuilder
struct AttachmentContentBuilder
```

## Overview

The `buildBlock` methods in this type create AttachmentContent instances based on the number and types of sources provided as parameters.

RealityKit calls this builder for you when SwiftUI annotates the `attachment` parameter of some RealityView initializers that have the `@AttachmentContentBuilder` annotation.

## Topics

### Type Methods

static func buildBlock() -> EmptyAttachmentContent

Creates an empty attachment content containing no statements.

static func buildBlock&lt;C>(C) -> C

Creates a single content result.

static func buildBlock&lt;each Content>(repeat each Content) -> TupleAttachmentContent&lt;(repeat each Content)>

Provides support for lists of Attachments to be created in parallel.

static func buildEither&lt;TrueContent, FalseContent>(first: TrueContent) -> ConditionalAttachmentContent&lt;TrueContent, FalseContent>

Provides support for “if” statements in multi-statement closures, producing conditional content for the “then” branch.

static func buildEither&lt;TrueContent, FalseContent>(second: FalseContent) -> ConditionalAttachmentContent&lt;TrueContent, FalseContent>

Provides support for “if-else” statements in multi-statement closures, producing conditional content for the “else” branch.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

static func buildIf&lt;Content>(Content?) -> Content?

Provides support for “if” statements in multi-statement closures, producing an optional view that is visible only when the condition evaluates to `true`.

static func buildLimitedAvailability(any AttachmentContent) -> some AttachmentContent

Provides support for “if” statements with `#available()` clauses in multi-statement closures, producing conditional content for the “then” branch, i.e. the conditionally-available branch.

## See Also

### Attachment types

protocol AttachmentContent

A type that provides content for an attachment content builder.

struct ConditionalAttachmentContent

struct EmptyAttachmentContent

A attachment content that doesn’t contain any content.

struct TupleAttachmentContent

struct AnyAttachmentContent

A type-erased attachment content.

