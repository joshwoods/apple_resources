

- Security
-  kSecCFErrorResourceSeal 

Global Variable

# kSecCFErrorResourceSeal

A key whose value is a Core Foundation object containing the part of the resource seal that had a problem.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecCFErrorResourceSeal: CFString
```

## Discussion

The `CodeResources` file that gets generated as part of the code signing process serves as the bundle’s seal. This file is a CFDictionary that contains a listing of all the files found within your bundle coupled with their respective hash values and a set of rule definitions. The type of object returned depends on which item in the dictionary had a problem. See macOS Code Signing In Depth for more information on the `CodeResources` file.

