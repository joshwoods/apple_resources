

- SwiftUI
- OpenURLAction
-  callAsFunction(\_:) 

Instance Method

# callAsFunction(\_:)

Opens a URL, following system conventions.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
func callAsFunction(_ url: URL)
```

## Parameters 

`url`  

The URL to open.

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the OpenURLAction structure that you get from the Environment, using a URL as an argument:

```
struct OpenURLExample: View {
    @Environment(\.openURL) private var openURL

    var body: some View {
        Button {
            if let url = URL(string: "https://www.example.com") {
                openURL(url) // Implicitly calls openURL.callAsFunction(url)
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

func callAsFunction(URL, completion: (Bool) -> Void)

Asynchronously opens a URL, following system conventions.

