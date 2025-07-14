

- QuickTime File Format
- Storing and sharing media with QuickTime files
-  Creating, copying, and disposing of atom containers 

# Creating, copying, and disposing of atom containers

Manage atoms in atom containers.

## Overview

Before you can add atoms to an atom container, you must first create the container by calling `QTNewAtomContainer`. The code sample shown in the following calls `QTNewAtomContainer` to create an atom container.

```
QTAtomContainer spriteData;
OSErr err
// Create an atom container to hold a sprite’s data.
err=QTNewAtomContainer (&spriteData);
```

When you have finished using an atom container, dispose of it by calling the `QTDisposeAtomContainer` function. The sample code shown in the following listing calls `QTDisposeAtomContainer` to dispose of the `spriteData` atom container.

```
if (spriteData)
    QTDisposeAtomContainer (spriteData);
```

## Topics

### Managing atoms

Creating new atoms

Create new atoms and insert them in a QT atom container.

Copying existing atoms

Copy existing atoms within an atom container.

Retrieving atoms from an atom container

Retrieve information about the types of a parent atom’s children, search for a specific atom, and retrieve a leaf atom’s data.

Modifying atoms

Modify attributes or data associated with an atom in an atom container.

Removing atoms from an atom container

Remove atoms from an atom container.

## See Also

### Building in QuickTime

Atoms

The basic data unit in a QuickTime file is the atom.

QT atoms and atom containers

An enhanced data structure that provide a more general-purpose storage format.

QuickTime movie files

The QuickTime file format describes the characteristics of QuickTime movie files.

