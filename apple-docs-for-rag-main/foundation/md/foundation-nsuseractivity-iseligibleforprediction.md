

- Foundation
- NSUserActivity
-  isEligibleForPrediction 

Instance Property

# isEligibleForPrediction

A Boolean value that determines whether Siri can suggest the user activity as a shortcut to the user.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 5.0+

``` source
var isEligibleForPrediction: Bool { get set }
```

## Discussion

To donate a user activity to Siri Shortcuts, set isEligibleForPrediction to true and make the user activity current. To make the user activity current, call the activity’s becomeCurrent() method, or assign it to the userActivity property on a UIViewController or UIResponder object. For more information, see Donating Shortcuts.

## See Also

### Donating to Siri Shortcuts

var suggestedInvocationPhrase: String?

A phrase suggested to the user when they create a shortcut.

var shortcutAvailability: INShortcutAvailabilityOptions

A set of defined contexts in which an intent or activity might be relevant to a user.

