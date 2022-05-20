# Process-Management-Exercise-Android-App
When the app is opened, the structure selected by default is the Pigman House

The Structure Name is actually a spinner widget. Tapping on it will show the list of structures. Selecting a structure (e.g. Merman House) will take you to Image 3

When the BUILD button is clicked, it does the following:
Disables the BUILD button / itself
Shows the Progress Bar
Launches necessary threads that take care of a Building Block Tile’s behaviour
Hides the Notification (if applicable)
You may use whatever method you wish to launch worker threads for the Building Block Tiles. Formally, a worker thread’s responsibility is as follows:
Sets a Building Block Tile’s visibility to INVISIBLE after a random delay
The delay ranges from 500 milliseconds to 5500 milliseconds
For example, Tile 1 waits for 751 milliseconds before making its tile INVISIBLE, while Tile 2 waits for 3847 milliseconds before making its tile invisible, and so on
Finds a way to properly update the progress bar

Once all Tiles have been processed, the following occurs:
The Progress Bar is hidden
The BUILD button is re-enabled
A pop-up Notification is shown
This pop-up Notification is NOT an actual Notification, it is simply a View Group that is already available in the provided layout
When the Notification appears, its Structure Image and Structure Description should change to match the currently shown Structure


Once the BUILD button is re-enabled, the spinner is also re-enabled with it
 When a user switches the selected Structure via the spinner, the Notification should disappear and all Building Block Tiles should reappear
 
 This holds true, even if the user were to re-select the previously built Structure (ie. Mushroom Museum).
 
