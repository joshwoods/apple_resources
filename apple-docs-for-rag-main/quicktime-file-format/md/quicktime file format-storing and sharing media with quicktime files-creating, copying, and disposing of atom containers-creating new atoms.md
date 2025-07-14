

- QuickTime File Format
- Storing and sharing media with QuickTime files
- Creating, copying, and disposing of atom containers
-  Creating new atoms 

Article

# Creating new atoms

Create new atoms and insert them in a QT atom container.

## Overview

You can use the `QTInsertChild` function to create new atoms and insert them in a QT atom container. The `QTInsertChild` function creates a new child atom for a parent atom. The caller specifies an atom type and atom ID for the new atom. If you specify a value of `0` for the atom ID, `QTInsertChild` assigns a unique ID to the atom.

`QTInsertChild` inserts the atom in the parent’s child list at the index specified by the index parameter; any existing atoms at the same index or greater are moved toward the end of the child list. If you specify a value of `0` for the index parameter, `QTInsertChild` inserts the atom at the end of the child list.

The code sample in the following listing creates a new QT atom container and calls `QTInsertChild` to add an atom. The resulting QT atom container is shown in the following figure. The offset value `10` is returned in the `firstAtom` parameter.

```
QTAtom firstAtom;
QTAtomContainer container;
OSErr err
err = QTNewAtomContainer (&container);
if (!err)
    err = QTInsertChild (container, kParentAtomIsContainer, 'abcd',
        1000, 1, 0, nil, &firstAtom);
```

The following figure shows a QT atom container after you insert an atom.

The following code sample calls `QTInsertChild` to create a second child atom. Because a value of `1` is specified for the index parameter, the second atom is inserted in front of the first atom in the child list; the index of the first atom is changed to `2`. The resulting QT atom container is shown in the following figure.

```
QTAtom secondAtom;

FailOSErr (QTInsertChild (container, kParentAtomIsContainer, 'abcd',
    2000, 1, 0, nil, &secondAtom));
```

The following figure shows a QT atom container after you insert a second atom.

You can call the `QTFindChildByID` function to retrieve the changed offset of the first atom that was inserted, as shown in the following example. In this example, the `QTFindChildByID` function returns an offset of `20`.

```
firstAtom = QTFindChildByID (container, kParentAtomIsContainer,  'abcd',
    1000, nil);
```

The following listing shows how the `QTInsertChild` function inserts a leaf atom into the atom container sprite. The new leaf atom contains a sprite image index as its data.

```
if ((propertyAtom = QTFindChildByIndex (sprite, kParentAtomIsContainer,
    kSpritePropertyImageIndex, 1, nil)) == 0)

    FailOSErr (QTInsertChild (sprite, kParentAtomIsContainer,
        kSpritePropertyImageIndex, 1, 1, sizeof(short),&imageIndex,
        nil));
```

## See Also

### Managing atoms

Copying existing atoms

Copy existing atoms within an atom container.

Retrieving atoms from an atom container

Retrieve information about the types of a parent atom’s children, search for a specific atom, and retrieve a leaf atom’s data.

Modifying atoms

Modify attributes or data associated with an atom in an atom container.

Removing atoms from an atom container

Remove atoms from an atom container.

