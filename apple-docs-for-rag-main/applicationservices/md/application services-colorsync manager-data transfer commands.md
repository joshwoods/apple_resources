

- Application Services
- ColorSync Manager
-  Data Transfer Commands 

# Data Transfer Commands

Specify commands for caller-supplied ColorSync data transfer functions.

## Overview

When your application calls the function CMFlattenProfile, any of the functions in the group Accessing Profile Elements, or the PostScript-related functions of type Working With PostScript, the selected CMM—or, for the `CMUnflattenProfile` function, the ColorSync Manager—calls the flatten function you supply to transform profile data. The call passes one of the command constants defined by this enumeration.

Your application provides a pointer to your ColorSync data transfer function as a parameter to the functions. The ColorSync Manager or the CMM calls your data transfer function, passing the command in the `command` parameter. For more information on the flatten function, see CMFlattenProfile.

## Topics

### Constants

var cmOpenReadSpool: Int

Directs the function to begin the process of reading data.

var cmOpenWriteSpool: Int

Directs the function to begin the process of writing data.

var cmReadSpool: Int

Directs the function to read the number of bytes specified by the `CMFlattenProcPtr` function’s `size` parameter.

var cmWriteSpool: Int

Directs the function to write the number of bytes specified by the `CMFlattenProcPtr` function’s `size` parameter.

var cmCloseSpool: Int

Directs the function to complete the data transfer.

