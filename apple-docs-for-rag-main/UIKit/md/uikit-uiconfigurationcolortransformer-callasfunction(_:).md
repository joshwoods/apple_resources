

- UIKit
- UIConfigurationColorTransformer
-  callAsFunction(\_:) 

Instance Method

# callAsFunction(\_:)

Calls the transform closure of the color transformer.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
func callAsFunction(_ input: UIColor) -> UIColor
```

## Discussion

Using this syntax, you can call the color transformer type as if it were a closure:

```
let alphaColorTransformer = UIConfigurationColorTransformer() { baseColor -> UIColor in
    return baseColor.withAlphaComponent(0.5)
}

let baseColor = UIColor.red
let modifiedColor = alphaColorTransformer(baseColor)
```

## See Also

### Calling the color transformer

let transform: (UIColor) -> UIColor

The transform closure of the color transformer.

