

- VisionKit
- ImageAnalyzer
-  ImageAnalyzer.Configuration 

Structure

# ImageAnalyzer.Configuration

A configuration that specifies the types of items and locales that the image analyzer recognizes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+macOS 13.0+visionOS 1.0+

``` source
struct Configuration
```

## Mentioned in 

Enabling Live Text interactions with images

## Overview

Create an `ImageAnalyzer.Configuration` structure to specify the criteria when analyzing an image. Then pass the configuration object to the `ImageAnalyzer` analyze(_:configuration:) or similar method to find the items you want.

## Topics

### Creating configurations

init(ImageAnalyzer.AnalysisTypes)

Creates a configuration that an image analyzer uses to find items.

let analysisTypes: ImageAnalyzer.AnalysisTypes

The types of items that the image analyzer looks for in the image.

struct AnalysisTypes

The types of items that an image analyzer looks for in an image.

### Recognizing languages

var locales: [String]

The languages to use in text items that the image analyzer recognizes.

