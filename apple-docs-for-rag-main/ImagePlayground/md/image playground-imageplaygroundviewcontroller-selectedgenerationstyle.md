

- Image Playground
- ImagePlaygroundViewController
-  selectedGenerationStyle 

Instance Property

# selectedGenerationStyle

Generation style to pre-select upong launching the playground among those in `allowedGenerationStyles`.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor @preconcurrency
var selectedGenerationStyle: ImagePlaygroundStyle { get set }
```

## Discussion

Use `ImagePlaygroundStyle.all` to check the list of all possible styles, and pass one of those.

## See Also

### Specifying the configuration of the playground

var allowedGenerationStyles: [ImagePlaygroundStyle]

A list of allowed generation styles to choose from in the playground.

var personalizationPolicy: ImagePlaygroundPersonalizationPolicy

The policy to apply when determining whether to include people in generated images.

enum ImagePlaygroundPersonalizationPolicy

A policy for enabling or disabling personalization in the system interface.

