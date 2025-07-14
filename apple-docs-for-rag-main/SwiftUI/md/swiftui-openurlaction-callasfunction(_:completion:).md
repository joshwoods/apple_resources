

- SwiftUI
- OpenURLAction
-  callAsFunction(\_:completion:) 

Instance Method

# callAsFunction(\_:completion:)

Asynchronously opens a URL, following system conventions.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func callAsFunction(
    _ url: URL,
    completion: @escaping (Bool) -> Void
)
```

## Parameters 

`url`  

The URL to open.

`completion`  

A closure the method calls after determining if it can open the URL, but possibly before fully opening the URL. The closure takes a Boolean value that indicates whether the method can open the URL.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the OpenURLAction structure that you get from the Environment, using a URL and a completion handler as arguments:

```
struct OpenURLExample: View {
    @Environment(\.openURL) private var openURL

    var body: some View {
        Button {
            if let url = URL(string: "https://www.example.com") {
                // Implicitly calls openURL.callAsFunction(url) { ... }
                openURL(url) { accepted in
                    print(accepted ? "Success" : "Failure")
                }
            }
        } label: {
            Label("Get Help", systemImage: "person.fill.questionmark")
        }
    }
}
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

## See Also

### Calling the action

func callAsFunction(URL)

Opens a URL, following system conventions.

