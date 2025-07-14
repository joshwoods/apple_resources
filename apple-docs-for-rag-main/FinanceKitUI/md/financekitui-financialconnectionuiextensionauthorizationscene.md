

- FinanceKitUI
-  FinancialConnectionUIExtensionAuthorizationScene 

Structure

# FinancialConnectionUIExtensionAuthorizationScene

Implement this scene to authorize your app’s Financial Connection

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
@MainActor @preconcurrency
struct FinancialConnectionUIExtensionAuthorizationScene where Content : View
```

## Overview

Your scene will be provided a `FinancialConnectionExtensionAuthorizationRequest`. Use this request to query parameters necessary for authentication, and callback when complete.

## Topics

### Initializers

init(content: () -> Content)

### Instance Properties

var body: some AppExtensionScene

The content and behavior of the scene’s user interface.

### Type Aliases

typealias Body

The type for this scene’s body.

## Relationships

### Conforms To

- AppExtensionScene
- FinancialConnectionUIExtensionScene
- Sendable

