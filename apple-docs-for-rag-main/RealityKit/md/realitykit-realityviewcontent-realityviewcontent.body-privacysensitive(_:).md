

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  privacySensitive(\_:) 

Instance Method

# privacySensitive(\_:)

Marks the view as containing sensitive, private user data.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func privacySensitive(_ sensitive: Bool = true) -> some View
```

## Discussion

SwiftUI redacts views marked with this modifier when you apply the `RedactionReasons/privacy` redaction reason.

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

