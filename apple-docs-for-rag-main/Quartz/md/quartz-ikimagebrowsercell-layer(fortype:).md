

- Quartz
- IKImageBrowserCell
-  layer(forType:) 

Instance Method

# layer(forType:)

Returns a layer for the specified position.

macOS 10.4+

``` source
func layer(forType type: String!) -> CALayer!
```

## Parameters 

`type`  

A string representing the layer location. See Cell Layer Positions for possible values.

## Return Value

The `CALayer` to display in the specified position.

## Discussion

Subclasses can override this method to add a Core Animation layer to the cell

