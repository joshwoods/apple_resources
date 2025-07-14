

- Core Services
- File Metadata
- MDQuery
-  Query Search Scope Keys 

API Collection

# Query Search Scope Keys

Specify the scope of a query’s search.

## Overview

These constants can be passed in the `scopeDirectories` array to the function `MDQuerySetSearchScope`.

## Topics

### Constants

let kMDQueryScopeHome: CFString!

Specifies that the query should be restricted to the volume and directory that contains the current user’s home directory.

let kMDQueryScopeComputer: CFString!

Specifies that the query should be restricted to all locally mounted volumes, plus the user’s home directory (which may be on a remote volume).

let kMDQueryScopeNetwork: CFString!

Specifies that the query should include all user mounted remote volumes.

let kMDQueryScopeAllIndexed: CFString!

Specifies that the search should be restricted to indexed, locally mounted volumes and indexed user mounted remote volumes, plus the user's home directory.

let kMDQueryScopeComputerIndexed: CFString!

Specifies that the search should be restricted to indexed, locally mounted volumes, plus the user's home directory (which may be on a remote volume).

let kMDQueryScopeNetworkIndexed: CFString!

Specifies that the search should include indexed user mounted remote volumes.

## See Also

### Notification Info Keys

Query Result Change Keys

Specify the items that have changed in the query results.

Result Relevance Sorting Key

Key used in a user notification’s description dictionary that indicates the relevance of a result.

