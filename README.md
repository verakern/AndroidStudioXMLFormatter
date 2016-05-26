# AndroidStudioXMLFormatter
A formatter for xml files in Android. Currently only rules for for layout files are defined.

This formatter expresses rules for formatting Android xml layout files according to my personal preferences.
Those are:
- root element has all xmlns, sorted alphabetically
1) id
2) style
3) layout_width
4) layout_height
5) layout_weight
6) all other layout_* attributes
7) all other attributes except what appears below
8) text attributes (textColor, etc.) with the actual text last
9) background
10) orientation
11) visibility
12)elevation
13) all other name space attributes, sorted alphabetically

If you want to use it you can import it in Android Studio 2.2 Preview 1 and higher by opening the Preferences (Command + ,), then going to Editor -> Code Style -> XML. Click the "Manage..." button and use the import feature.

If you are on a lower version of Android Studio, you can go to ~/Library/Preferences and select the Android Studio version you are currently using. If you find a folder called codestyles, paste the xml file there. If there is no such folder, create it and then paste the file. Restart Android Studio, go to the formatter and the file should show up in the drop down next to “Manage...”.

The rules defined in this file are shown on the "Arrangement" - tab.

Please note that using this file will overwrite your settings on the other tabs as well!
