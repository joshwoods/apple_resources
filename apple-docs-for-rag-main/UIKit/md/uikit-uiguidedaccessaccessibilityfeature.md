

- UIKit
-  UIGuidedAccessAccessibilityFeature 

Structure

# UIGuidedAccessAccessibilityFeature

Constants that describe accessibility features for Guided Access.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct UIGuidedAccessAccessibilityFeature
```

## Topics

### Constants

static var assistiveTouch: UIGuidedAccessAccessibilityFeature

The AssistiveTouch accessibility feature.

static var grayscaleDisplay: UIGuidedAccessAccessibilityFeature

The Grayscale accessibility feature.

static var invertColors: UIGuidedAccessAccessibilityFeature

The Smart Invert accessibility feature.

static var voiceOver: UIGuidedAccessAccessibilityFeature

The VoiceOver assistive app.

static var zoom: UIGuidedAccessAccessibilityFeature

The Zoom accessibility feature.

### Initializers

init(rawValue: UInt)

Creates a Guided Access accessibility feature with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Guided Access

static func configureForGuidedAccess(features: UIGuidedAccessAccessibilityFeature, enabled: Bool, completionHandler: (Bool, (any Error)?) -> Void)

Enables or disables the specified accessibility features while using Guided Access.

enum Code

Error codes for Guided Access.

