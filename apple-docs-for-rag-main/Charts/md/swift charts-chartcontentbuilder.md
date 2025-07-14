

- Swift Charts
-  ChartContentBuilder 

Structure

# ChartContentBuilder

A result builder that you use to compose the contents of a chart.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
struct ChartContentBuilder
```

## Overview

This Result Builder combines any number of ChartContent instances into a single composite instance, including support for conditionals.

You don’t call the methods of the result builder directly. Instead, Swift uses them to combine the elements that you declare in any closure that has the `@ChartContentBuilder` attribute. In particular, you rely on this behavior when you declare the `content` inside a Chart initializer like init(content:).

## Topics

### Building chart content

static func buildPartialBlock&lt;T>(first: T) -> T

Builds a partial result from a single, first component.

Deprecated

static func buildPartialBlock(accumulated: some ChartContent, next: some ChartContent) -> some ChartContent

Builds a partial result by combining an accumulated component and a new component.

Deprecated

static func buildBlock() -> some ChartContent

Produces empty chart content.

### Building conditionally

static func buildIf&lt;T>(T?) -> T?

Builds a partial result that’s conditionally present.

static func buildEither&lt;T1, T2>(first: T1) -> BuilderConditional&lt;T1, T2>

Builds a partial result from a condition that’s true.

static func buildEither&lt;T1, T2>(second: T2) -> BuilderConditional&lt;T1, T2>

Builds a partial result from a condition that’s false.

### Building with conditional availability

static func buildLimitedAvailability(some ChartContent) -> AnyChartContent

Builds a partial result that propagates or erases type information outside a compiler-controlled availability check.

### Supporting types

struct BuilderConditional

A conditional result from a result builder.

### Type Methods

static func buildBlock&lt;each C>(repeat each C) -> some ChartContent

Builds a result from multiple components.

static func buildBlock&lt;C>(C) -> C

Builds a result from a single component.

static func buildExpression&lt;Content>(Content) -> Content

## See Also

### Charts

Creating a chart using Swift Charts

Make a chart by combining chart building blocks in SwiftUI.

Visualizing your app’s data

Build complex and interactive charts using Swift Charts.

struct Chart

A SwiftUI view that displays a chart.

protocol ChartContent

A type that represents the content that you draw on a chart.

struct Plot

A mechanism for grouping chart contents into a single entity.

