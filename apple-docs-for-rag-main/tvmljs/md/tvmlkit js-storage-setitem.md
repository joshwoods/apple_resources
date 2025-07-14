

- TVMLKit JS
- Storage
-  setItem 

Instance Method

# setItem

Associates the given data with the given key.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 4.0+Safari Mobile 3.0+

**tvOS**

``` source
void setItem(
    in String key, 
    in String data
);
```

**Safari Desktop, Safari Mobile**

``` source
void setItem(
    DOMString key, 
    DOMString data
);
```

## Parameters 

`key`  

A `String` object containing the key associated with the data to be saved.

`data`  

A `String` object containing the data to be stored.

## Discussion

The `setItem` function first checks whether the given key already exists in the storage. If it does not, then the key and associated value are stored. If the key already exists and the data in storage is different than the data being passed, the new data is saved to storage.

## See Also

### Accessing Key-Value Pair Information

clear

Removes all instances of key-value pairs from the storage list.

getItem

Retrieves the data associated with the specified key.

key

Returns the key located in the specified location.

length

The number of key-value pairs currently in the storage list.

removeItem

Deletes a key and all associated data from storage.

