

- WebKit JS
- WebKitCSSKeyframesRule
-  insertRule 

# insertRule

Adds a keyframe rule to the collection of keyframes.

``` source
void insertRule (in DOMString rule);
```

## Parameters 

`rule`  

A string representing a selector and keyframe, where the selector is a percentage or keyword and the keyframe is a block. The string must follow the format for keyframe blocks in the @-webkit-keyframes CSS rule.

## See Also

### Changing Rules

deleteRule

Removes a keyframe rule from the collection of keyframes.

findRule

Returns the keyframe rule for the specified selector.

