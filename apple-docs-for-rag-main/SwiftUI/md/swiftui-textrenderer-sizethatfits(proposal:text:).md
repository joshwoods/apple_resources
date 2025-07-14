

- SwiftUI
- TextRenderer
-  sizeThatFits(proposal:text:) 

Instance Method

# sizeThatFits(proposal:text:)

Returns the size of the text in `proposal`. The provided `text` proxy value may be used to query the sizing behavior of the underlying text layout.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func sizeThatFits(
    proposal: ProposedViewSize,
    text: TextProxy
) -> CGSize
```

**Required** Default implementation provided.

## Discussion

The default implementation of this function returns `text.size(proposal)`.

## Default Implementations

### TextRenderer Implementations

func sizeThatFits(proposal: ProposedViewSize, text: TextProxy) -> CGSize

Returns the size of the text in `proposal`. The provided `text` proxy value may be used to query the sizing behavior of the underlying text layout.

