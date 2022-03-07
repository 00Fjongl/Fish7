# Fish7
### What is this?
This HTML file is designed to automatically create browsing history entries. While it shares similarities with "history flooding" tools, it allows for more in-depth control over how entries are created. When used properly, the browsing history of a user may turn out to be more convincing than if a history flooding tool had been used.
### Features
* Customizable intervals
* Customizable site list
* Site randomization
* Multiple sessions
* Monitors for troubleshooting
* Export as bookmarklet
### Using the menus
##### What do the buttons do?
The **Begin** button creates a new tab using information from the rest of the text boxes. Hold CTRL while clicking to create tabs more quickly. Websites are automatically selected from the site list at random. Bookmarklets and data URIs will not function by default.  
  
Holding Shift while clicking on it will also create a new tab. However, it will only visit the URLs in the order they are listed, execute any bookmarklets on the menu, and end after visiting all URLs in the list.  
  
The **Terminate** button closes all of the tabs created by the file. This only works if the user did not hold Shift upon beginning.  
  
The box in the upper-right corner exports the entire menu, including its current site list, history, and settings, as a bookmarklet. Additionally, exported settings can be loaded by replacing the entire site list with the bookmarklet, then holding Shift and clicking on **Begin**.
##### What do the options do?
There are options to set how quickly a tab switches websites, to set when a tab should close itself (if ever), and to replace frequent words or phrases in the site list. The options are as follows:
Option | Effect | Parameters
------ | ------ | ----------
`Rate\|ms` | Sets how quickly a tab switches websites. | Set the interval in milliseconds, without punctuation. Numbers expressed in scientific E notation are also accepted (e.g. 1e4 for 10000).
`Timeout\|ms` | Sets when a tab should close itself. | Leave empty to have the tab never close itself. Otherwise, the parameters are the same as with `Rate\|ms`.
`Random hash` | Adds a random ending to the end of every URL. Does not change the content of the website, but allows revisited sites to be registered more often in the browsing history.
`Replace` and `with` | Replaces keywords, phrases, or other content that appears in the site list. Useful for changing all `https` to `http` and vice versa. | Enter what's being replaced in `Replace`. Enter what it should be replaced with in `with`. Hold Shift and press Enter to replace.
##### What are the larger boxes for?
The left box contains the site list that will be processed. The right box is a menu that will show what was entered last, separated for each tab. The area directly above the two boxes tracks all sites that the file attempted to visit.  
  
URLs in the right box can be edited. Pressing Enter after changing the site will cause the associated tab to visit the new URL, acting as an override.
* If no text is supplied upon entering, then its tab will close.  
* If the text is not a website, then Google will be used to search for it instead.
##### Can I resize the boxes?
Currently, only the large menu boxes can be resized. There are small handles at the bottom-right corners of the left menu and the upper menu, to resize horizontally and resize vertically.
##### Working with multiple sessions
Each generated tab will keep track of the site list, interval, and all other settings at the time of being opened. Modifying any of the settings afterward will not affect previous tabs. This allows for the creation of multiple tabs, or sessions, that use different settings.
