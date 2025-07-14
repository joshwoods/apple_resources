

- XCUIAutomation
- XCUIElement
-  hover() 

Instance Method

# hover()

Moves the pointer over the element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSXcode 16.3+

``` source
@MainActor
func hover()
```

## Discussion

If the element exists within a scrollable view but is offscreen, XCTest attempts to scroll the element onscreen before moving the cursor over the element.

