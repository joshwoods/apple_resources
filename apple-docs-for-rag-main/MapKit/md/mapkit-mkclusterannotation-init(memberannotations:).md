

- MapKit
- MKClusterAnnotation
-  init(memberAnnotations:) 

Initializer

# init(memberAnnotations:)

Creates a cluster annotation with the specified individual annotations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(memberAnnotations: [any MKAnnotation])
```

## Parameters 

`memberAnnotations`  

The annotations to group together as a single entity.

## Return Value

An initialized MKClusterAnnotation object or `nil` if the object could not be created.

