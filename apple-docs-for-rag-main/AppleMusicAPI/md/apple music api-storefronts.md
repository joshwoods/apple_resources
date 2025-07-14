

- Apple Music API
-  Storefronts 

Object

# Storefronts

A resource object that represents a storefront, an Apple Music and iTunes Store territory that the content is available in.

Apple Music 1.0+

``` source
object Storefronts
```

## Properties

`id`

`string`

 (Required) 

The identifier for the storefront.

`type`

`string`

 (Required) 

This value must always be `storefronts`.

Value: `storefronts`

`href`

`string`

 (Required) 

The relative location for the storefront resource.

`attributes`

Storefronts.Attributes

The attributes for the storefront.

## Discussion

For the specification of language tags, see Language Codes in iTunes Package Music Specification.

## Topics

### Related Objects

object Storefronts.Attributes

The attributes for the storefronts resource.

