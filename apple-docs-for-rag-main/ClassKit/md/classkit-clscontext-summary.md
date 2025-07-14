

- ClassKit
- CLSContext
-  summary 

Instance Property

# summary

An optional, user-visible description of the context.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+

``` source
var summary: String? { get set }
```

## Discussion

The Schoolwork app may display this string to help the user understand the kinds of activities the context provides.

Localize the summary string, and limit its length to 4,000 characters.

## See Also

### Identifying the context

var identifier: String

A string that uniquely identifies a context among its siblings.

var title: String

The name of the context as it appears to users.

var thumbnail: CGImage?

An optional thumbnail image associated with the context.

