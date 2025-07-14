

- TipKit
- Tips
-  showTipsForTesting(\_:) 

Type Method

# showTipsForTesting(\_:)

Show specified tips regardless of their display rule eligibility or display frequency status for UI testing of certain tips.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func showTipsForTesting(_ tips: [any Tip.Type])
```

## Parameters 

`tips`  

Array of tips to show regardless of their display rule eligibility.

## Overview

This function can also be called with the launch argument `-com.apple.TipKit.ShowTips FindTrailheadTip,SlopeProfileTip`.

TipKit’s display override testing functions have the following precedence:

| Priority | Testing function |
|----|----|
| First | showTipsForTesting(_:) |
| Second | hideTipsForTesting(_:) |
| Third | showAllTipsForTesting() |
| Fourth | hideAllTipsForTesting() |

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
            Tips.showTipsForTesting([FindTrailheadTip.self, SlopeProfileTip.self])
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

static func showAllTipsForTesting()

Show all tips regardless of their display rule eligibility or display frequency status for UI testing of tips.

static func hideAllTipsForTesting()

Hide all tips regardless of their display rule eligibility for UI testing without tips.

static func hideTipsForTesting([any Tip.Type])

Hide specified tips regardless of their display rule eligibility for UI testing without certain tips.

static func resetDatastore() throws

Resets the tips’ datastore to the initial state for re-testing tip display rules and eligibility.

