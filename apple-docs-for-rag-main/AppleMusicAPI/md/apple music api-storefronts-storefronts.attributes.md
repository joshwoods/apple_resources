

- Apple Music API
- Storefronts
-  Storefronts.Attributes 

Object

# Storefronts.Attributes

The attributes for the storefronts resource.

Apple Music 1.0+

``` source
object Storefronts.Attributes
```

## Properties

`defaultLanguageTag`

`string`

 (Required) 

The default supported RFC4646 language tag for the storefront.

`explicitContentPolicy`

`string`

 (Required) 

Attribute indicating the level that this storefront can display explicit content.

Possible Values: `allowed, opt-in, prohibited`

`name`

`string`

 (Required) 

The localized name of the storefront.

`supportedLanguageTags`

`[string]`

 (Required) 

The supported RFC4646 language tags for the storefront.

