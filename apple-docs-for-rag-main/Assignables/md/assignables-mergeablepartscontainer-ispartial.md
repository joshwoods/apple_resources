

- Assignables
- MergeablePartsContainer
-  isPartial 

Instance Property

# isPartial

Documents are considered partial when they are reconstituted missing one or more of their associated document part IDs. When a document is considered partial it is expected that we shouldn’t be able to both read or write to the parts that the document has neither been reconstituted or merged with.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
var isPartial: Bool { get }
```

**Required**

