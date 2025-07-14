

- Core Services
- Carbon Core
- Unicode Utilities
-  Key State Entry Formats 

# Key State Entry Formats

Indicate the format for dead-key state records.

## Overview

These constants are used in `UCKeyStateRecord` structures to indicate the format for dead-key state records.

## Topics

### Constants

var kUCKeyStateEntryTerminalFormat: Int

Specifies that the entry format is that of a structure of type UCKeyStateEntryTerminal. Use this format for simple (single) dead-key states, as in the U.S. keyboard layout.

var kUCKeyStateEntryRangeFormat: Int

Specifies that the entry format is that of a structure of type UCKeyStateEntryRange. Use this format for complex (multiple) dead-key states, as in the hex input and Hangul input keyboard layouts.

