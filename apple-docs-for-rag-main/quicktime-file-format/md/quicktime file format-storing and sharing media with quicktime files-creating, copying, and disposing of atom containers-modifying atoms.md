

- QuickTime File Format
- Storing and sharing media with QuickTime files
- Creating, copying, and disposing of atom containers
-  Modifying atoms 

Article

# Modifying atoms

Modify attributes or data associated with an atom in an atom container.

## Overview

`TextQuickTime` provides functions that you can call to modify attributes or data associated with an atom in an atom container. To modify an atom’s ID, you call the function `QTSetAtomID`.

You use the `QTSetAtomData` function to update the data associated with a leaf atom in an atom container. The `QTSetAtomData` function replaces a leaf atom’s data with new data. The code sample in the following listing calls `QTFindChildByIndex` to determine whether an atom container contains a sprite’s visible property. If so, the sample calls `QTSetAtomData` to replace the atom’s data with a new visible property.

```
QTAtom propertyAtom;

// if the atom isn’t in the container, add it
if ((propertyAtom = QTFindChildByIndex (sprite, kParentAtomIsContainer,
    kSpritePropertyVisible, 1, nil)) == 0)
    FailOSErr (QTInsertChild (sprite, kParentAtomIsContainer,
        kSpritePropertyVisible, 1, 0, sizeof(short), visible, nil))

// if the atom is in the container, replace its data
else
    FailOSErr (QTSetAtomData (sprite, propertyAtom, sizeof(short),
        visible));
```

## See Also

### Managing atoms

Creating new atoms

Create new atoms and insert them in a QT atom container.

Copying existing atoms

Copy existing atoms within an atom container.

Retrieving atoms from an atom container

Retrieve information about the types of a parent atom’s children, search for a specific atom, and retrieve a leaf atom’s data.

Removing atoms from an atom container

Remove atoms from an atom container.

