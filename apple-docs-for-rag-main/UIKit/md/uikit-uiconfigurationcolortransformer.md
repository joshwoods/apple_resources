

- UIKit
-  UIConfigurationColorTransformer 

Structure

# UIConfigurationColorTransformer

A transformer that generates a modified output color from an input color.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct UIConfigurationColorTransformer
```

## Overview

A color transformer takes an input color and modifies it to produce a different output color. For example, you might have a color transformer that returns a grayscale or reduced alpha version of the input color.

Because color transformers can use the same base input color to produce a number of variants of that color, you can create different appearances for different states of your views.

## Topics

### Creating a color transformer

init((UIColor) -> UIColor)

Creates a color transformer with the specified closure.

static let grayscale: UIConfigurationColorTransformer

Creates a color transformer that generates a grayscale version of the color.

static let preferredTint: UIConfigurationColorTransformer

A color transformer that returns the preferred system accent color.

static let monochromeTint: UIConfigurationColorTransformer

A color transformer that returns the color with a monochrome tint.

### Calling the color transformer

let transform: (UIColor) -> UIColor

The transform closure of the color transformer.

func callAsFunction(UIColor) -> UIColor

Calls the transform closure of the color transformer.

