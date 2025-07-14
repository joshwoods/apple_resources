

- TV Services
- TVTopShelfItem
-  init(identifier:) 

Initializer

# init(identifier:)

Creates a top shelf item with the specified identifier.

tvOS 13.0+

``` source
init(identifier: String)
```

## Parameters 

`identifier`  

The string you use to identify this item. This string must be unique among all of the items you ever return from your app. Never recycle identifiers.

## Return Value

An empty item object.

## Discussion

After creating the item object, call the setImageURL(_:for:) method to assign an image and one or more actions to the item. Include the item object in the TVTopShelfContent object you return from your extension.

