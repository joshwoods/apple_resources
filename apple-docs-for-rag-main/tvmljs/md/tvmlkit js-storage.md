

- TVMLKit JS
-  Storage 

Class

# Storage

An object used to store key-value-pair information.

TVMLKit JSWebKit JStvOS 9.0+Safari Desktop 10.0+Safari Mobile 3.0+

``` source
interface Storage
```

## Overview

You cannot create a new instance of the `Storage` class. The available instances in TVMLKit JS are `localStorage` and `sessionStorage`. Local storage writes the data to the disk, while session storage writes the data to the memory only. Any data written to the session storage is purged when your app exits.

## Topics

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

setItem

Associates the given data with the given key.

## See Also

### Data Storage and Retrieval

Binding JSON data to TVML documents

Create full-fledged TVML documents by using data binding and queries on simplified TVML files.

XMLHttpRequest

An object used to retrieve data from a URL.

DataItem

An object used to create observable objects from JSON objects for data binding.

DataSource

An interface that allows the system to detect and respond to changes in your data.

LoadIndexesRequest

A request created when the loadindexes event is triggered.

