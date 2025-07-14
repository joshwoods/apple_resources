

- Create ML Components
- ObjectDetectionMetrics
-  extractLabels(from:) 

Type Method

# extractLabels(from:)

Extracts all the labels from a list of annotations.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
static func extractLabels(from annotations: [ObjectDetectionAnnotation]) -> Set
```

## Parameters 

`annotations`  

A list of annotations.

## Return Value

A set of all the labels present in the annotations.

