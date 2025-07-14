

- MapKit JS
- mapkit.Padding
-  mapkit.Padding 

Initializer

# mapkit.Padding

Creates a padding object and initializes its inset margin properties.

MapKit JS 5.0+

``` source
new mapkit.Padding(
 optional PaddingConstructorOptions options,
 optional number top,
 optional number right,
 optional number bottom,
 optional number left
);
```

## Parameters 

`top`  

An object literal with the keys defined in PaddingConstructorOptions, or a list of four numbers that represent inset margin values. The numbers represent the top, right, bottom, and left insets, respectively.

## Discussion

Create mapkit.Padding by passing in four numbers that represent the inset values from the top, right, bottom, and left edges. Alternatively, use an object literal instance with the keys defined in PaddingConstructorOptions.

The following examples show two ways to create padding:

```
// example 1: 4 numbers
map.padding = new mapkit.Padding(
    10, // top inset
    10, // right inset
    10, // bottom inset
    10) // left inset

// example 2: object literal conforming to PaddingConstructorOptions
map.padding = new mapkit.Padding({top: 10, right: 10, bottom: 10, left:10})

```

## See Also

### Creating padding

PaddingConstructorOptions

Initial values of the edge insets for padding.

