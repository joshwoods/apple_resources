

- SwiftUI
-  SafeAreaRegions 

Structure

# SafeAreaRegions

A set of symbolic safe area regions.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
struct SafeAreaRegions
```

## Topics

### Getting safe area regions

static let all: SafeAreaRegions

All safe area regions.

static let container: SafeAreaRegions

The safe area defined by the device and containers within the user interface, including elements such as top and bottom bars.

static let keyboard: SafeAreaRegions

The safe area matching the current extent of any software keyboard displayed over the view content.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Staying in the safe areas

func ignoresSafeArea(SafeAreaRegions, edges: Edge.Set) -> some View

Expands the safe area of a view.

func safeAreaInset(edge:alignment:spacing:content:)

Shows the specified content beside the modified view.

func safeAreaPadding(_:)

Adds the provided insets into the safe area of this view.

func safeAreaPadding(Edge.Set, CGFloat?) -> some View

Adds the provided insets into the safe area of this view.

