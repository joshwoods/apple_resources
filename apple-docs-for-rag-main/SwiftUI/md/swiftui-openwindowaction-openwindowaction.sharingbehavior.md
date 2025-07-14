

- SwiftUI
- OpenWindowAction
-  OpenWindowAction.SharingBehavior 

Structure

# OpenWindowAction.SharingBehavior

macOS 15.0+

``` source
struct SharingBehavior
```

## Topics

### Type Properties

static let requested: OpenWindowAction.SharingBehavior

The window will be shared if there is an available sharing session and the person using your app confirms the offer to share. The window will be opened regardless of whether sharing succeeds.

static let required: OpenWindowAction.SharingBehavior

The window will be shared if there is an available sharing session and the person using your app confirms the offer to share. The window will only be opened if sharing succeeds.

## Relationships

### Conforms To

- Sendable

