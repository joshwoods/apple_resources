

- SwiftUI
- TextSelectionAffinity
-  TextSelectionAffinity.upstream 

Case

# TextSelectionAffinity.upstream

An upstream selection affinity. In this case, the cursor is associated with the character immediately before it.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
case upstream
```

## Discussion

In the context of our example `hello|مرحبا`, with an upstream affinity, the cursor would be associated with the “o” from “hello”. If you were to type in English, the characters would continue to be added after the “o” in “hello”.

