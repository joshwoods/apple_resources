

- SwiftUI
- View
-  privacySensitive(\_:) 

Instance Method

# privacySensitive(\_:)

Marks the view as containing sensitive, private user data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func privacySensitive(_ sensitive: Bool = true) -> some View
```

## Discussion

SwiftUI redacts views marked with this modifier when you apply the privacy redaction reason.

```
struct BankAccountView: View {
    var body: some View {
        VStack {
            Text("Account #")

            Text(accountNumber)
                .font(.headline)
                .privacySensitive() // Hide only the account number.
        }
    }
}
```

## See Also

### Redacting private content

Designing your app for the Always On state

Customize your watchOS app’s user interface for continuous display.

func redacted(reason: RedactionReasons) -> some View

Adds a reason to apply a redaction to this view hierarchy.

func unredacted() -> some View

Removes any reason to apply a redaction to this view hierarchy.

var redactionReasons: RedactionReasons

The current redaction reasons applied to the view hierarchy.

var isSceneCaptured: Bool

The current capture state.

struct RedactionReasons

The reasons to apply a redaction to data displayed on screen.

