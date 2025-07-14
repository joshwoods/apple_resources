

- TVMLKit JS
- Storage
-  getItem 

Instance Method

# getItem

Retrieves the data associated with the specified key.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 4.0+Safari Mobile 3.0+

**tvOS**

``` source
String getItem(
    in String key
);
```

**Safari Desktop, Safari Mobile**

``` source
getter DOMString? getItem(
    DOMString key
);
```

## Parameters 

`key`  

A `String` object containing the key being searched for.

## Return Value

A `String` object containing the data associated with the passed key.

## Discussion

The `getItem` function retrieves the data associated with the given key. If the key does not exist, the function returns `null`.

## See Also

### Accessing Key-Value Pair Information

clear

Removes all instances of key-value pairs from the storage list.

key

Returns the key located in the specified location.

length

The number of key-value pairs currently in the storage list.

removeItem

Deletes a key and all associated data from storage.

setItem

Associates the given data with the given key.

