

- RoomPlan
- StructureBuilder
-  init(options:) 

Initializer

# init(options:)

Creates a structure builder using the specified options.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 16.0–1.0Deprecated

``` source
init(options: StructureBuilder.ConfigurationOptions)
```

## Parameters 

`options`  

An option set to customize the captured structure.

## Discussion

Pass the `StructureBuilder/ConfigurationOptions/beautifyObjects` option to enhance the look of the output for the captured structure, or (`[]`) to omit capture post-processing.

## See Also

### Creating a structure builder

typealias ConfigurationOptions

Options that configure a structure builder.

