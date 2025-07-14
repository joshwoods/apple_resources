

- XCUIAutomation
- XCUIApplication
-  resetAuthorizationStatus(for:) 

Instance Method

# resetAuthorizationStatus(for:)

Resets the authorization status for a protected resource.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+tvOS 13.4+visionOS 1.0+watchOS 6.2+Xcode 16.3+

``` source
@MainActor
func resetAuthorizationStatus(for resource: XCUIProtectedResource)
```

## Parameters 

`resource`  

A system resource that requires user authorization to access.

## See Also

### Resetting authorization status

enum XCUIProtectedResource

A system resource that requires user authorization to access.

