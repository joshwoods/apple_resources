

- XCUIAutomation
-  XCUIAccessibilityAuditIssue 

Class

# XCUIAccessibilityAuditIssue

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Xcode 16.3+

``` source
class XCUIAccessibilityAuditIssue
```

## Topics

### Type and description

var auditType: XCUIAccessibilityAuditType

var compactDescription: String

var detailedDescription: String

### UI element

var element: XCUIElement?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Performing an accessibility audit

func performAccessibilityAudit(for: XCUIAccessibilityAuditType, ((XCUIAccessibilityAuditIssue) throws -> Bool)?) throws

struct XCUIAccessibilityAuditType

