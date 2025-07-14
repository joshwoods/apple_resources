

- Security
-  AuthorizationRights 

Type Alias

# AuthorizationRights

An authorization item set designated to represent a set of rights.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AuthorizationRights = AuthorizationItemSet
```

## Discussion

The argument value of each item in the set is as defined for the specific right it belongs to. Argument values may not contain pointers so they remain portable between different address spaces. This set is actually an instance of an AuthorizationItemSet.

