

- SwiftUI
-  PresentationDetent 

Structure

# PresentationDetent

A type that represents a height where a sheet naturally rests.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct PresentationDetent
```

## Topics

### Getting built-in detents

static let large: PresentationDetent

The system detent for a sheet at full height.

static let medium: PresentationDetent

The system detent for a sheet that’s approximately half the height of the screen, and is inactive in compact height.

### Creating custom detents

static func custom&lt;D>(D.Type) -> PresentationDetent

A custom detent with a calculated height.

static func fraction(CGFloat) -> PresentationDetent

A custom detent with the specified fractional height.

static func height(CGFloat) -> PresentationDetent

A custom detent with the specified height.

struct Context

Information that you use to calculate the presentation’s height.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Configuring a sheet’s height

func presentationDetents(Set&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet.

func presentationDetents(Set&lt;PresentationDetent>, selection: Binding&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet, giving you programmatic control of the currently selected detent.

func presentationContentInteraction(PresentationContentInteraction) -> some View

Configures the behavior of swipe gestures on a presentation.

func presentationDragIndicator(Visibility) -> some View

Sets the visibility of the drag indicator on top of a sheet.

protocol CustomPresentationDetent

The definition of a custom detent with a calculated height.

struct PresentationContentInteraction

A behavior that you can use to influence how a presentation responds to swipe gestures.

