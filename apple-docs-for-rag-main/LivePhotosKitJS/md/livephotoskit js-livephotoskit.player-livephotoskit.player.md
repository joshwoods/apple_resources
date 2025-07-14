

- LivePhotosKit JS
- LivePhotosKit.Player
-  LivePhotosKit.Player 

Initializer

# LivePhotosKit.Player

Creates `LivePhotosKit.Player` objects.

LivePhotosKit JS 1.0+

``` source
new targetElement(
 HTMLElement targetElement,
 Object options
);
```

## Parameters 

`targetElement`  

The target DOM element to be decorated with additional properties and methods that allow it to act as the Player of Live Photos. If a target element is not passed, a `HTMLDivElement` will be created and used instead.

`options`  

An object containing keys and values for any subset of the public writable properties of Player. If provided, the values provided in this object will be used instead of the default values for those Player properties.

## Return Value

The target element passed in, modified with additional properties and methods to allow it to act as a Live Photo player. If no target element was provided, then a new `HTMLDivElement` will be created and returned with Live Photo player functionality.

