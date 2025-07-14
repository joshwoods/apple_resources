

- ActivityKit
- ActivityAttributes
-  ContentState 

Associated Type

# ContentState

The associated type that describes the dynamic content of a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
associatedtype ContentState : Decodable, Encodable, Hashable
```

**Required**

## Discussion

The dynamic data of a Live Activity that’s encoded by `ContentState` can’t exceed 4KB.

