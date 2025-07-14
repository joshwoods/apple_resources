

- SwiftUI
-  FittedPresentationSizing 

Structure

# FittedPresentationSizing

The size of the presentation is dictated by the ideal size of the content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct FittedPresentationSizing
```

## Overview

The presentation is sized by proposing `nil` in the horizontal and vertical dimensions.

See Also

fitted

## Relationships

### Conforms To

- PresentationSizing
- Sendable

## See Also

### Supporting types

struct AutomaticPresentationSizing

The default presentation sizing, appropriate for the platform.

struct FormPresentationSizing

The size is appropriate for forms and slightly less wide than`.page`

struct PagePresentationSizing

The size is roughly the size of a page of paper, appropriate for informational or compositional content.

