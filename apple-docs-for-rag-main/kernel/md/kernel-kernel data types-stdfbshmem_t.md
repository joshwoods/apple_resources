

- Kernel
- Kernel Data Types
-  StdFBShmem_t 

# StdFBShmem_t

macOS 10.6+

``` source
struct StdFBShmem_t {
    ...
};
```

## Topics

### Instance Properties

cursor

cursorLoc

cursorObscured

If this is true, the cursor has been obscured and cursorShow should not be 0. The cursor will be shown again the next time it is moved.

cursorRect

The region that the cursor image currently occupies in software cursor mode.

cursorSema

cursorShow

The cursor is displayed when cursorShow is 0.

cursorSize

frame

hardwareCursorActive

hardwareCursorCapable

hardwareCursorShields

hotSpot

oldCursorRect

reservedB

reservedC

saveRect

screenBounds

shieldFlag

When this is set to true the cursor will not be displayed in the region specified by shieldRect.

shieldRect

shielded

structSize

vblCount

vblDelta

vblDeltaMeasured

vblDeltaReal

vblDrift

vblTime

The time of the most recent vertical blanking.

version

