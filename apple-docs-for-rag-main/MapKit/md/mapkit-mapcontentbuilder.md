

- MapKit
-  MapContentBuilder 

Structure

# MapContentBuilder

A result builder that creates map content from closures you provide.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@resultBuilder
struct MapContentBuilder
```

## Overview

The buildBlock(_:) methods in this type create MapContent instances based on the number and types of sources you provide as parameters.

You don’t use this type directly. Instead, SwiftUI annotates the `content` parameter of the various `MapView` initializers with the `@MapContentBuilder` annotation, implicitly calling this builder for you.

## Topics

### Map content builders

static func buildBlock() -> EmptyMapContent

Creates an empty map content block that contains no statements.

static func buildBlock&lt;C>(C) -> C

Creates a map content block that contains a single content result.

### Conditionally building map content

static func buildEither&lt;TrueContent, FalseContent>(first: TrueContent) -> _ConditionalMapContent&lt;TrueContent, FalseContent>

Compares content in a multistatement closure, resulting in use of the conditional content if the first argument you provide evaluates to  true.

static func buildEither&lt;TrueContent, FalseContent>(second: FalseContent) -> _ConditionalMapContent&lt;TrueContent, FalseContent>

Compares content in a multistatement closure, resulting in use of the conditional content if the second argument you provide evaluates to true.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the map content builder.

static func buildIf&lt;Content>(Content?) -> Content?

Compares content in a multistatement closure, that produces an optional view that’s visible if the argument you provide evaluates to true.

static func buildLimitedAvailability(any MapContent) -> some MapContent

Provides support for “if” statements with “available” macro clauses in multi-statement closures, producing conditional content for the “then” branch, such the conditionally-available branch.

### Type Methods

static func buildBlock&lt;each Content>(repeat each Content) -> TupleMapContent&lt;(repeat each Content)>

## See Also

### Protocols

protocol DynamicMapContent

A  type of view that generates views from an underlying collection of data.

protocol MapContent

A protocol used to construct map content such as controls, markers, and annotations.

struct MapContentView

A view that contains content that displays on a map at a specific position, and that responds to specific interactions you specify.

