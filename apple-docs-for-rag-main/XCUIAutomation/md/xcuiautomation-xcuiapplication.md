

- XCUIAutomation
-  XCUIApplication 

Class

# XCUIApplication

A proxy that can launch, monitor, and terminate a test application.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
class XCUIApplication
```

## Overview

Use this class to launch, monitor, and terminate your app in a UI test. Use wait(for:timeout:) to launch your app and wait for it to reach an expected state before you check test conditions.

## Topics

### Creating an application proxy

init()

Creates a proxy for the application that’s configured as the Target Application in Xcode’s target settings.

init(bundleIdentifier: String)

Creates a proxy for an application for the specified bundle identifier.

init(url: URL)

Creates a proxy for the application at the specified file system URL.

### Launching the application

func launch()

Launches the application.

var launchArguments: [String]

The arguments that pass to the application on launch.

var launchEnvironment: [String : String]

The environment variables that pass to the application on launch.

func open(URL)

Launches the application by URL.

### Activating the application

func activate()

Activates the application.

### Terminating the application

func terminate()

Terminates any running instance of the application.

### Determining application state

var state: XCUIApplication.State

The most recent state of the application.

enum State

The possible states of an application during UI testing.

### Waiting for an application state

func wait(for: XCUIApplication.State, timeout: TimeInterval) -> Bool

Waits for the application to reach the specified state or timeout.

### Resetting authorization status

func resetAuthorizationStatus(for: XCUIProtectedResource)

Resets the authorization status for a protected resource.

enum XCUIProtectedResource

A system resource that requires user authorization to access.

### Performing an accessibility audit

func performAccessibilityAudit(for: XCUIAccessibilityAuditType, ((XCUIAccessibilityAuditIssue) throws -> Bool)?) throws

struct XCUIAccessibilityAuditType

class XCUIAccessibilityAuditIssue

## Relationships

### Inherits From

- XCUIElement

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- XCUIElementAttributes
- XCUIElementSnapshotProviding
- XCUIElementTypeQueryProvider
- XCUIScreenshotProviding

