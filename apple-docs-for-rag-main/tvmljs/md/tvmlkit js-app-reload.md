

- TVMLKit JS
- App
-  reload 

Instance Method

# reload

Reloads the app.

tvOS 9.0+

``` source
void reload(
    in Object options, 
    in optional Object reloadData
);
```

## Parameters 

`options`  

The options used to determine when the app is reloaded. This parameter is a dictionary with a key-value pair. The key can have the value `when`. The value can have the values `onResume` or `now`.

`reloadData`  

An optional, developer-defined object that contains information about the current app state.

## Discussion

This function reloads the initial TVMLKit JS file without quitting the app. The optional `reloadData` parameter enables you to capture and restart the app in its current state. If the `reloadData` parameter is not present, the app is restarted in its initial state.

