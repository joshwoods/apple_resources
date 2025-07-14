

- LivePhotosKit JS
- LivePhotosKit
-  LIVEPHOTOSKIT_LOADED 

# LIVEPHOTOSKIT_LOADED

An event that is fired when LivePhotosKit JS is loaded.

LivePhotosKit JS 1.0+

``` source
const String LIVEPHOTOSKIT_LOADED;
```

## Discussion

This event is fired when `livephotoskit.js` is loaded asynchronously. It always has the value `livephotoskitloaded`.

For example, log this event as follows.

```
document.addEventListener('livephotoskitloaded', function(e) {
  console.log('Loaded LivePhotosKit JS');
});
```

## See Also

### Constants

VERSION

The version of LivePhotosKit JS.

