

- QuickTime File Format
- Media data atom types
- Text media
-  Hypertext and wired text 

Article

# Hypertext and wired text

Store hypertext in a text track sample atom.

## Overview

Hypertext is used as an action that takes you to a Web URL; like a Web URL, it appears blue and underlined. Hypertext is stored in a text track sample atom stream as type `'htxt'`. The same mechanism is used to store wired actions linked to text strings. A text string can be wired to act as a hypertext link when clicked or to perform any defined QuickTime wired action when clicked. For details on wired actions, see Wired action grammar.

The data stored is a `QTAtomContainer`. The root atom of hypertext in this container is a wired-text atom of type `'wtxt'`. This is the parent for all individual hypertext objects.

For each hypertext item, the parent atom is of type `'htxt'`. This is the atom container atom type. Two children of this atom that define the offset of the hypertext in the text stream are:

```
kRangeStart         strt // unsigned long
kRangeEnd           end  // unsigned long
```

Child atoms of the parent atom are the events of type `kQTEventType` and the ID of the event type. The children of these event atoms follow the same format as other wired events.

```
kQTEventType, (kQTEventMouseClick, kQTEventMouseClickEnd,
                    kQTEventMouseClickEndTriggerButton,
                    kQTEventMouseEnter, kQTEventMouseExit)
...
kTextWiredObjectsAtomType, 1
    kHyperTextItemAtomType, 1..n
         kRangeStart, 1
            long
        kRangeEnd, 1
            long

    kAction     // The known range of track movie sprite actions

```

## See Also

### Storing text data

Text sample description

An atom that defines how to interpret text media data.

Text media information atom ('text')

An atom that contains information about text media.

Text sample data

An atom that contains text data.

