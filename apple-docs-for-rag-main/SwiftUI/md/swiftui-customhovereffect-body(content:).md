

- SwiftUI
- CustomHoverEffect
-  body(content:) 

Instance Method

# body(content:)

Defines the effect produced by this effect.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
func body(content: Self.Content) -> Self.Body
```

**Required** Default implementation provided.

## Parameters 

`content`  

An empty effect you use to compose the custom effect.

## Return Value

A custom effect.

## Discussion

You implement this method to describe a custom effect to apply to a view. `content` is an empty effect you use to build your effect, which will later be applied to a View, or combined with other `CustomHoverEffect`s.

## Default Implementations

### CustomHoverEffect Implementations

func body(content: Self.Content) -> Self.Body

Defines the effect produced by this effect.

