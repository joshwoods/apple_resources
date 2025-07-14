

- Contacts
- CNLabeledValue
-  identifier 

Instance Property

# identifier

A unique identifier for the labeled value object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var identifier: String { get }
```

## Discussion

It is recommended that you use the `identifier` when searching for a previously known labeled value object in a re-fetched contact. The identifier can be persisted between the app launches.

