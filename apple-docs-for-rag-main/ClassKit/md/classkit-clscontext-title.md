

- ClassKit
- CLSContext
-  title 

Instance Property

# title

The name of the context as it appears to users.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var title: String { get set }
```

## Discussion

The title that you choose appears to teachers exactly as you store it. If your app works in many locales, localize the title. The framework doesn’t do that for you automatically.

## See Also

### Identifying the context

var identifier: String

A string that uniquely identifies a context among its siblings.

var summary: String?

An optional, user-visible description of the context.

var thumbnail: CGImage?

An optional thumbnail image associated with the context.

