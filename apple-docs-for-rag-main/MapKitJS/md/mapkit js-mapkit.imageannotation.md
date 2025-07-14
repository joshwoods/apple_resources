

- MapKit JS
-  mapkit.ImageAnnotation 

Class

# mapkit.ImageAnnotation

A customized annotation with image resources that you provide.

MapKit JS 5.0+

``` source
interface mapkit.ImageAnnotation
```

## Overview

There are times when you want to customize the look of an annotation. The easiest way to do that is to use a mapkit.ImageAnnotation object, which lets you specify your own image resources. Minimally, all you need to provide is a URL to your asset (such as a PNG or JPEG image).

To make your image look crisp on Retina displays, provide URLs to the Retina versions of your asset. You may want to define the anchor of your asset with anchorOffset.

The shape of your icon might affect the placement of the callout. You can modify the position of the callout with calloutOffset.

## Topics

### Creating an image annotation

mapkit.ImageAnnotation

Creates an image annotation with a URL to its image and a coordinate.

ImageAnnotationConstructorOptions

An object containing options for creating an image annotation.

### Retrieving the image URL

url

An object containing URLs for the image assets in multiple resolutions.

## Relationships

### Inherited By

- mapkit.Annotation

