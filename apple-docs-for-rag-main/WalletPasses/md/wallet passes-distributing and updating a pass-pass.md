

- Wallet Passes
-  Distributing and updating a pass 

Article

# Distributing and updating a pass

Distribute a pass to your users or update an existing pass.

## Overview

There are three ways you can distribute a pass:

- Add a pass from an app or App Clip.

- Provide a download on a web page for one pass or a bundle containing multiple passes.

- Send a pass as an attachment in an email.

In your app or App Clip, add a PKAddPassButton to show that a pass is available. When the user taps the button, show a PKAddPassesViewController for the pass.

On your website, show an Add to Apple Wallet button. Download the pass when the user clicks the button. For more information on displaying the button, see the Add to Apple Wallet Guidelines.

Update a pass by distributing a new version of the pass with the same pass identifier and serial number. For more information on the pass identifier and serial number, see the `passTypeIdentifier` and `serialNumber` keys of the Pass object.

You can optionally provide a web service to update the contents of a user’s pass, such as changing the time for an event. For more information about implementing a pass update web service, see Adding a Web Service to Update Passes.

### Create a bundle of passes

Provide a bundle of passes to enable your user to download multiple passes at once. To create the pass bundle:

1.  Create a `.zip` file containing the `.pkpass` files for the passes that are part of the bundle.

2.  Change the extension of the `.zip` file to `.pkpasses`.

You can distribute a bundle of passes the same way you distribute a single pass. The MIME type for a bundle of passes is “`application/vnd.apple.pkpasses"`.

Note

You can have up to 10 passes or 150 MB for a bundle of passes.

## See Also

### Essentials

Creating the Source for a Pass

Create the directory structure and add source files and images to define a pass.

Building a Pass

Build a distributable pass.

object Pass

An object that represents a pass.

