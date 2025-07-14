

- TipKit
- Tips
-  showAllTipsForTesting() 

Type Method

# showAllTipsForTesting()

Show all tips regardless of their display rule eligibility or display frequency status for UI testing of tips.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func showAllTipsForTesting()
```

## Overview

This function can also be called with the launch argument `-com.apple.TipKit.ShowAllTips 1`.

TipKit’s display override testing functions have the following precedence:

| Priority | Testing function |
|----|----|
| first | showTipsForTesting(_:) |
| second | hideTipsForTesting(_:) |
| third | showAllTipsForTesting() |
| fourth | hideAllTipsForTesting() |

```
import SwiftUI
import TipKit

@main
struct LandmarkTips: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
    }

    init() {
        setupTips()
    }

    // Configure tips in the app.
    func setupTips() {
        do {
            #if DEBUG
            Tips.showAllTipsForTesting()
            #endif

            try Tips.configure()
        }
        catch {
            print("Error initializing TipKit \(error.localizedDescription)")
        }
    }
}
```

## See Also

### Testing

static func showTipsForTesting([any Tip.Type])

Show specified tips regardless of their display rule eligibility or display frequency status for UI testing of certain tips.

static func hideAllTipsForTesting()

Hide all tips regardless of their display rule eligibility for UI testing without tips.

static func hideTipsForTesting([any Tip.Type])

Hide specified tips regardless of their display rule eligibility for UI testing without certain tips.

static func resetDatastore() throws

Resets the tips’ datastore to the initial state for re-testing tip display rules and eligibility.

