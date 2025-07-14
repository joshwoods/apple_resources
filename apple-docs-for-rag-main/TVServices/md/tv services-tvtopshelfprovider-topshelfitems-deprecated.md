

- TV Services
- TVTopShelfProvider
-  topShelfItems Deprecated

Instance Property

# topShelfItems

Returns an array of content items to be displayed.

tvOS 9.0–13.0Deprecated

``` source
var topShelfItems: [TVContentItem] { get }
```

**Required**

Deprecated

TVTopShelfProvider has been replaced by TVTopShelfContentProvider

## Discussion

If the value is an empty array, the system falls back to the static image provided with the app.

## See Also

### Implementing TV Services Extension Properties

var topShelfStyle: TVTopShelfContentStyle

The user interface style that should be used to display the content items.

**Required**

Deprecated

enum TVTopShelfContentStyle

An enumerated type used to specify the style in which you want your content to be displayed.

Deprecated

