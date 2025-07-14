

- DeveloperToolsSupport
-  PreviewRegistry 

Protocol

# PreviewRegistry

A protocol that the system uses to locate previews at runtime.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol PreviewRegistry
```

## Overview

Preview macros make use of this protocol on your behalf. Don’t use it directly. Instead, use one of the preview macros, like Preview(_:body:).

Important

If you define a preview registry directly, the behavior is undefined.

## Topics

### Type Properties

static var column: Int

**Required**

static var fileID: String

**Required**

static var line: Int

**Required**

static var preview: Preview

**Required** Default implementation provided.

Deprecated

### Type Methods

static func makePreview() throws -> Preview

**Required**

## See Also

### Preview Registration

struct Preview

A base type that preview macros use to create previews.

enum PreviewLayout

A size constraint for a preview.

struct PreviewTrait

Customizations that you can apply to a preview.

