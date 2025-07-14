

- AdAttributionKit
- Postback
-  reengagementOpenURLParameter 

Type Property

# reengagementOpenURLParameter

A string that represents the query parameter that AdAttributionKit appends to the URL to indicate that a reengagement has occurred.

iOS 18.0+iPadOS 18.0+Mac Catalyst

``` source
static var reengagementOpenURLParameter: String { get }
```

## Mentioned in 

Receiving ad attributions and postbacks

## Discussion

When your advertised app receives a universal link, determine whether it came from an AdAttributionKit reengagement by checking the query parameters for a key containing this string, as the example below shows:

```
   func isAdAttributionKitReengagementURL(url: URL) -> Bool {
       guard let components = URLComponents(url: url, resolvingAgainstBaseURL: true),
             let queryItems = components.queryItems else {
           return false
       }
       return queryItems.contains { $0.name == Postback.reengagementOpenURLParameter }
   }
```

