

- UIKit
- UIImage
-  init(systemName:variableValue:configuration:) 

Initializer

# init(systemName:variableValue:configuration:)

Creates an image object that contains a system symbol image with the configuration and variable value you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
convenience init?(
    systemName name: String,
    variableValue: Double,
    configuration: UIImage.Configuration? = nil
)
```

## Parameters 

`name`  

The name of the system symbol image.

`variableValue`  

The value the system uses to customize the image content, between `0` and `1`.

`configuration`  

The image configuration the system applies to the image.

## Return Value

The object containing the image variant that matches the specified configuration data, or `nil` if no suitable image was found.

## Discussion

Use this method to retrieve system-defined symbol images. To retrieve a custom symbol image you store in an asset catalog, use the init(named:in:variableValue:configuration:) method instead.

This method checks the system caches for an image with the specified name and returns the variant of that image that’s best suited for the configuration you specify. If a matching image object isn’t in the cache, this method creates the image from the system symbol image.

The system may purge cached image data at any time to free up memory. Purging occurs only for unused images that are in the cache.

To look up the names of system symbol images, download the SF Symbols app from Apple Design Resources.

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

convenience init?(named: String, in: Bundle?, variableValue: Double, configuration: UIImage.Configuration?)

Creates an image by using the name, configuration, and variable value you specify.

init?(named: String)

Creates an image object from the specified named asset.

convenience init(imageLiteralResourceName: String)

Returns the image object for the specified resource.

init?(systemName: String, withConfiguration: UIImage.Configuration?)

Creates an image object that contains a system symbol image with the specified configuration.

init?(systemName: String, compatibleWith: UITraitCollection?)

Creates an image object that contains a system symbol image appropriate for the specified traits.

init?(systemName: String)

Creates an image object that contains a system symbol image.

convenience init(resource: ImageResource)

Building high-performance lists and collection views

Improve the performance of lists and collections in your app with prefetching and image preparation.

