

- Swift Charts
-  BuilderConditional 

Structure

# BuilderConditional

A conditional result from a result builder.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct BuilderConditional
```

## Overview

Don’t use this type directly. The result builders defined by the framework, like ChartContentBuilder and AxisContentBuilder, use it as part of the building process.

## Relationships

### Conforms To

- AxisContent

  Conforms when `TrueContent` conforms to `AxisContent` and `FalseContent` conforms to `AxisContent`.

- AxisMark

  Conforms when `TrueContent` conforms to `AxisMark` and `FalseContent` conforms to `AxisMark`.

- ChartContent

  Conforms when `TrueContent` conforms to `ChartContent` and `FalseContent` conforms to `ChartContent`.

- Copyable

