

- Foundation
- NSUserActivity
-  suggestedInvocationPhrase 

Instance Property

# suggestedInvocationPhrase

A phrase suggested to the user when they create a shortcut.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var suggestedInvocationPhrase: String? { get set }
```

## Discussion

The system displays the suggested invocation phrase to the user when they create the shortcut. Use a short, memorable phrase, such as “Soup time”.

Note

To access the suggestedInvocationPhrase property, import the *Intents* framework.

## See Also

### Donating to Siri Shortcuts

var isEligibleForPrediction: Bool

A Boolean value that determines whether Siri can suggest the user activity as a shortcut to the user.

var shortcutAvailability: INShortcutAvailabilityOptions

A set of defined contexts in which an intent or activity might be relevant to a user.

