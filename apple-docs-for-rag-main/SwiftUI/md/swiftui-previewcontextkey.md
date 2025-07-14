

- SwiftUI
-  PreviewContextKey 

Protocol

# PreviewContextKey

A key type for a preview context.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
protocol PreviewContextKey
```

## Overview

The default value is `nil`.

## Topics

### Setting a default

static var defaultValue: Self.Value

The default value of the key.

**Required**

associatedtype Value

The type of the value returned by the key.

**Required**

## See Also

### Setting a context

func previewContext&lt;C>(C) -> some View

Declares a context for the preview.

protocol PreviewContext

A context type for use with a preview.

