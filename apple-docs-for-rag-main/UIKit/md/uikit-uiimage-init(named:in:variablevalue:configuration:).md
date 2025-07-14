

- UIKit
- UIImage
-  init(named:in:variableValue:configuration:) 

Initializer

# init(named:in:variableValue:configuration:)

Creates an image by using the name, configuration, and variable value you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
convenience init?(
    named name: String,
    in bundle: Bundle? = nil,
    variableValue: Double,
    configuration: UIImage.Configuration? = nil
)
```

## Parameters 

`name`  

The name of the image asset or file.

`bundle`  

The bundle that contains the image file or asset catalog.

`variableValue`  

The value the system uses to customize the image content, between `0` and `1`.

`configuration`  

The image configuration the system applies to the image.

## Return Value

An object that contains the image variant that matches the configuration data; otherwise, `nil` if the system didn’t find a suitable image.

## Discussion

When searching the asset catalog, this method prefers an asset containing a symbol image over an asset with the same name containing a bitmap image. Because the system supports symbol images in iOS 13 or later, you may include both types of assets in the same asset catalog. In iOS 12 or earlier, the system automatically chooses the bitmap image.

You can’t use this method to load system symbol images; use the init(systemName:variableValue:configuration:) method instead.

This method checks the system caches for an image object with the name you specify, and returns the variant of that image that best matches the trait collection you specify. If a matching image object isn’t in the cache, this method creates the image from an available asset catalog or loads the image from disk.

The system may purge cached image data at any time to free up memory. Purging occurs only for unused images that are in the cache.

## See Also

### Loading and caching images

Providing images for different appearances

Supply image resources appropriate for light and dark appearances and for high-contrast environments.

Configuring and displaying symbol images in your UI

Create scalable images that integrate with your app’s text, and adjust the appearance of those images dynamically.

Creating custom symbol images for your app

Create, organize, and annotate symbol images using SF Symbols.

init?(named: String, in: Bundle?, compatibleWith: UITraitCollection?)

Creates an image object using the named image asset that’s compatible with the specified trait collection.

init?(named: String, in: Bundle?, with: UIImage.Configuration?)

Creates an image by using the named image asset that’s compatible with the configuration you specify.

init?(named: String)

Creates an image object from the specified named asset.

convenience init(imageLiteralResourceName: String)

Returns the image object for the specified resource.

init?(systemName: String, withConfiguration: UIImage.Configuration?)

Creates an image object that contains a system symbol image with the specified configuration.

convenience init?(systemName: String, variableValue: Double, configuration: UIImage.Configuration?)

Creates an image object that contains a system symbol image with the configuration and variable value you specify.

init?(systemName: String, compatibleWith: UITraitCollection?)

Creates an image object that contains a system symbol image appropriate for the specified traits.

init?(systemName: String)

Creates an image object that contains a system symbol image.

convenience init(resource: ImageResource)

Building high-performance lists and collection views

Improve the performance of lists and collections in your app with prefetching and image preparation.

