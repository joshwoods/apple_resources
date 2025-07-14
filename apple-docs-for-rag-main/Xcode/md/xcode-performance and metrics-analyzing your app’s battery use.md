

- Xcode
- Performance and metrics
-  Analyzing your app’s battery use 

Article

# Analyzing your app’s battery use

Increase the available use time for your app on a single battery charge by reducing your appʼs power consumption.

## Overview

The Battery Usage pane in the Xcode Organizer shows a breakdown of the appʼs foreground and background power use, giving you a starting place to optimize power consumption.

The top graph shows the on-screen use, and the percentage of battery used during a 24-hour period while the app is in the foreground and the device isnʼt connected to power.

The bottom graph shows the background battery use during the same 24-hour period.

Clicking on a bar for a previous version shows a comparison of battery use to the right of the graphs. The zoomed-in section above shows an example of this data. The percentage values for each version are followed by a category breakdown. Larger values are shown in bold for easier comparison.

The power use categories are:

- Audio: Used to play audio in your app

- Networking: Used for networking

- Processing: Used by the CPU and GPU

- Display: Used to show the application UI

- Bluetooth: Used for Bluetooth

- Location: Used for location tracking within your app

- Camera: Used by the camera within your app

- Torch: Used for the flashlight

- NFC: Used for NFC within your app

- Other: A combination of the power in the above categories thatʼs too small to show in the list and any other power use

