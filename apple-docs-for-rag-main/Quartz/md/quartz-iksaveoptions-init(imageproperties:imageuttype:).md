

- Quartz
- IKSaveOptions
-  init(imageProperties:imageUTType:) 

Initializer

# init(imageProperties:imageUTType:)

Initializes a save options accessory pane for the provided image properties and uniform type identifier.

macOS 10.5+

``` source
init!(
    imageProperties: [AnyHashable : Any]!,
    imageUTType: String!
)
```

## Parameters 

`imageProperties`  

A dictionary of image properties.

`imageUTType`  

A string that specifies a uniform type identifier, such as `JPEG`. See Uniform Type Identifiers Overview.

## Return Value

The initialized object.

## See Also

### Creating A Save Options Accessory View

func addAccessoryView(to: NSSavePanel!)

Adds `IKSaveOptions` accessory view to a `NSSavePanel`.

