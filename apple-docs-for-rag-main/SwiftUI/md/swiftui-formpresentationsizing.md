

- SwiftUI
-  FormPresentationSizing 

Structure

# FormPresentationSizing

The size is appropriate for forms and slightly less wide than`.page`

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct FormPresentationSizing
```

## Overview

On iOS, `.form` sizing enforces a platform-defined floor for the vertical and horizontal dimensions. On macOS, no floor is enforced, however a maximum proposed height is derived from the presenter height. To achieve presentations outside of these bounds, see `PresentationSizing.fitted` or implement your own custom PresentationSizing.

See Also

form

## Relationships

### Conforms To

- PresentationSizing
- Sendable

## See Also

### Supporting types

struct AutomaticPresentationSizing

The default presentation sizing, appropriate for the platform.

struct FittedPresentationSizing

The size of the presentation is dictated by the ideal size of the content.

struct PagePresentationSizing

The size is roughly the size of a page of paper, appropriate for informational or compositional content.

