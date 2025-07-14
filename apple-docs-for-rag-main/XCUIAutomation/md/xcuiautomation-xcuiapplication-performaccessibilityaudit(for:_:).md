

- XCUIAutomation
- XCUIApplication
-  performAccessibilityAudit(for:\_:) 

Instance Method

# performAccessibilityAudit(for:\_:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+Xcode 16.3+

``` source
@MainActor @nonobjc @preconcurrency
func performAccessibilityAudit(
    for auditTypes: XCUIAccessibilityAuditType = .all,
    _ issueHandler: ((XCUIAccessibilityAuditIssue) throws -> Bool)? = nil
) throws
```

## See Also

### Performing an accessibility audit

struct XCUIAccessibilityAuditType

class XCUIAccessibilityAuditIssue

