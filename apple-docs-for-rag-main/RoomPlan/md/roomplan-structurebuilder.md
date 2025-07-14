

- RoomPlan
-  StructureBuilder 

Class

# StructureBuilder

An object that combines multiple scan sessions into a single captured result.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 16.0–1.0Deprecated

``` source
class StructureBuilder
```

## Mentioned in 

Scanning the rooms of a single structure

## Overview

This class in conjunction with CapturedStructure enables an app to export a 3D model that consists of multiple CapturedRoom instances. First, combine the rooms into a single captured result by calling capturedStructure(from:). Then, generate a 3D model of the whole structure by calling export(to:metadataURL:modelProvider:exportOptions:).

## Topics

### Creating a structure builder

init(options: StructureBuilder.ConfigurationOptions)

Creates a structure builder using the specified options.

typealias ConfigurationOptions

Options that configure a structure builder.

### Building a captured structure

func capturedStructure(from: [CapturedRoom]) async throws -> CapturedStructure

Combines the argument captured rooms into a single unit.

### Interpreting build errors

enum BuildError

Errors that can occur capturedStructure merging processing.

## See Also

### 3D Asset Output

Providing custom models for captured rooms and structure exports

Enhance the look of an exported 3D model by substituting object bounding boxes with detailed 3D renditions.

class RoomBuilder

An object that generates a 3D asset from room-capture data.

struct USDExportOptions

Options that determine the underlying data format of a scan export.

