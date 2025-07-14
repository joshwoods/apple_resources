

- XCUIAutomation
-  XCUIAccessibilityAuditType 

Structure

# XCUIAccessibilityAuditType

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Xcode 16.3+

``` source
struct XCUIAccessibilityAuditType
```

## Topics

### Accessibility audit type creation

init(rawValue: UInt64)

### Accessibility audit types

static var action: XCUIAccessibilityAuditType

static var all: XCUIAccessibilityAuditType

static var contrast: XCUIAccessibilityAuditType

static var dynamicType: XCUIAccessibilityAuditType

static var elementDetection: XCUIAccessibilityAuditType

static var hitRegion: XCUIAccessibilityAuditType

static var parentChild: XCUIAccessibilityAuditType

static var sufficientElementDescription: XCUIAccessibilityAuditType

static var textClipped: XCUIAccessibilityAuditType

static var trait: XCUIAccessibilityAuditType

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

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

### Performing an accessibility audit

func performAccessibilityAudit(for: XCUIAccessibilityAuditType, ((XCUIAccessibilityAuditIssue) throws -> Bool)?) throws

class XCUIAccessibilityAuditIssue

