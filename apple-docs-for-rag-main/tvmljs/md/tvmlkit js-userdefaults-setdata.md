

- TVMLKit JS
- UserDefaults
-  setData 

Instance Method

# setData

Stores the data for a given key.

tvOS 10.0+

``` source
void setData(
    in String key, 
    in String data
);
```

## Parameters 

`key`  

The key for the data to be stored.

`data`  

The data to be stored.

## Discussion

You can set the `data` parameter to `null` to remove the data associated with the key.

## See Also

### Modifying User Defaults

getData

Returns the data associated with a particular key.

removeData

Removes the data associated with a particular key.

