

- TVMLKit JS
- Storage
-  key 

Instance Method

# key

Returns the key located in the specified location.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 10.0+Safari Mobile 10.0+

**tvOS**

``` source
String key(
    in int index
);
```

**Safari Desktop, Safari Mobile**

``` source
DOMString? key(
    unsigned long index
);
```

## Parameters 

`index`  

The location of the key to be retrieved.

## Return Value

The found key.

## Discussion

If the value in the `index` parameter is greater than the number of key-value pairs currently in the storage list, this function returns `null`.

## See Also

### Accessing Key-Value Pair Information

clear

Removes all instances of key-value pairs from the storage list.

getItem

Retrieves the data associated with the specified key.

length

The number of key-value pairs currently in the storage list.

removeItem

Deletes a key and all associated data from storage.

setItem

Associates the given data with the given key.

