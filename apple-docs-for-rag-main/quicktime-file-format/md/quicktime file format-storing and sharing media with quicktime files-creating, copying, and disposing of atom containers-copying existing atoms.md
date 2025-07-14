

- QuickTime File Format
- Storing and sharing media with QuickTime files
- Creating, copying, and disposing of atom containers
-  Copying existing atoms 

Article

# Copying existing atoms

Copy existing atoms within an atom container.

## Overview

QuickTime provides several functions for copying existing atoms within an atom container. The `QTInsertChildren` function inserts a container of atoms as children of a parent atom in another atom container. The following figure shows two example QT atom containers, A and B.

The following code sample calls `QTFindChildByID` to retrieve the offset of the atom in container A. Then, the code sample calls the `QTInsertChildren` function to insert the atoms in container B as children of the atom in container A. The following figure shows what container A looks like after the atoms from container B have been inserted.

```
QTAtom targetAtom;

targetAtom = QTFindChildByID (containerA, kParentAtomIsContainer,  'abcd',
    1000, nil);

FailOSErr (QTInsertChildren (containerA, targetAtom, containerB));
```

The following figure shows a QT atom container after insert child atoms.

In the following listing, the `QTInsertChild` function inserts a parent atom into the atom container `theSample`. Then, the code calls `QTInsertChildren` to insert the container `theSprite` into the container `theSample`. The parent atom is `newSpriteAtom`.

```
FailOSErr (QTInsertChild (theSample, kParentAtomIsContainer,
    kSpriteAtomType, spriteID, 0, 0, nil, &newSpriteAtom));

FailOSErr (QTInsertChildren (theSample, newSpriteAtom, theSprite));
```

QuickTime provides three other functions you can use to manipulate atoms in an atom container. The `QTReplaceAtom` function replaces an atom and its children with a different atom and its children. You can call the `QTSwapAtoms` function to swap the contents of two atoms in an atom container; after swapping, the ID and index of each atom remains the same. The `QTCopyAtom` function copies an atom and its children to a new atom container.

## See Also

### Managing atoms

Creating new atoms

Create new atoms and insert them in a QT atom container.

Retrieving atoms from an atom container

Retrieve information about the types of a parent atom’s children, search for a specific atom, and retrieve a leaf atom’s data.

Modifying atoms

Modify attributes or data associated with an atom in an atom container.

Removing atoms from an atom container

Remove atoms from an atom container.

