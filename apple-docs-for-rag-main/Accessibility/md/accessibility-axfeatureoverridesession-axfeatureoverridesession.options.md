

- Accessibility
- AXFeatureOverrideSession
-  AXFeatureOverrideSession.Options 

Structure

# AXFeatureOverrideSession.Options

Options indicating which Accessibility features will be turned on or off when an override session is held by your app.

iOS 18.2+iPadOS 18.2+

``` source
struct Options
```

## Topics

### Initializers

init(rawValue: UInt)

### Type Properties

static var grayscale: AXFeatureOverrideSession.Options

static var invertColors: AXFeatureOverrideSession.Options

static var voiceControl: AXFeatureOverrideSession.Options

static var voiceOver: AXFeatureOverrideSession.Options

static var zoom: AXFeatureOverrideSession.Options

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

