

- SwiftUI
- PresentationDetent
- PresentationDetent.Context
-  subscript(dynamicMember:) 

Instance Subscript

# subscript(dynamicMember:)

Returns the value specified by the keyPath from the environment.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
subscript(dynamicMember keyPath: KeyPath) -> T { get }
```

## Overview

This uses the environment from where the sheet is shown, not the environment where the presentation modifier is applied.

