# Fish-7
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
The **Begin** button creates a new tab using information from the rest of the text boxes. Hold CTRL while clicking to create tabs more quickly.  
Holding Shift while clicking on **Begin** will also create a new tab. However, it will visit the URLs in the order they are listed, execute any bookmarklets on the menu, and end after visiting all URLs in the list.  
The **Terminate** button closes all of the tabs created by the file. This only works if the user did not hold Shift when beginning.
The box in the upper-right corner exports the entire menu, including its current site list, history, and settings, as a bookmarklet.
##### What do the options do?
There are options to set how quickly a tab switches websites, to set when a tab should close itself (if ever), and to replace frequent words or phrases in the site list. The options are as follows:
Option | Effect | Parameters
------ | ------ | ----------
`Rate\|ms` | Set how quickly a tab switches websites. | Set the interval in milliseconds, without punctuation. Numbers expressed in scientific E notation are also accepted (e.g. 1e4 for 10000).
`Timeout\|ms` | Set when a tab should close itself. | Leave empty to have the tab never close itself. Otherwise, the parameters are the same as with `Rate\|ms`.
`Random hash` | Add a random ending to the end of every URL. Does not change the content of the website, but allows revisited sites to be registered more often in the browsing history.
`replace` and `with` | Replace keywords, phrases, or other content that appears in the site list. Useful for changing all `https` to `http` and vice versa. | Enter what's being replaced in `replace`. Enter what it should be replaced with in `with`. Hold Shift and press Enter to replace.
##### What are the larger boxes for?
The left box contains the site list that will be processed. The right box is a menu that will show what was entered last, separated for each tab. The area directly above the two boxes tracks all sites that the file attempted to visit.  
URLs in the right box can be edited. Pressing Enter after changing the site will cause the associated tab to visit the new URL, acting as an override.  
* If no text is supplied upon entering, then the tab will close.  
* If the text is not a website, then Google will be used to search for it instead.
