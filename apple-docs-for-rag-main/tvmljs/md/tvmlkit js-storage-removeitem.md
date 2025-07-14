

- TVMLKit JS
- Storage
-  removeItem 

Instance Method

# removeItem

Deletes a key and all associated data from storage.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 4.0+Safari Mobile 3.0+

**tvOS**

``` source
void removeItem(
    in String key
);
```

**Safari Desktop, Safari Mobile**

``` source
void removeItem(
    DOMString key
);
```

## Parameters 

`key`  

A `String` object containing the key being searched for.

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

setItem

Associates the given data with the given key.

