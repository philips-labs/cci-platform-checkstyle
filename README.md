# cci-platform-checkstyle

## Local Setup
NOTE: These setups are one time pulls. We do not anticipate the styling document to change frequently, but if you are seeing build failures due to checkstyle please pull the checkstyle XML again.

### Intellij
* Navigate to _File_ -> _Settings_ -> _Plugins_, search `checkstyle` and install the "Checkstyle-IDEA" plugin
* Navigate to _File_ -> _Settings_ -> _Tools_ -> _Checkstyle_
* In the _Configuration File_ section, click on the "+"
* For _Description_ type `CCI Platform`
* Pulling the checkstyle XML
  * In a browser navigate [here](https://github.com/philips-internal/cci-platform-checkstyle/blob/main/checkstyle.xml)
  * Click on the "Raw" button
  * Copy the link the address bar
  * Back in Intellij, click on the "Use a checkstyle file accessable via HTTP" button
  * Fill in the corresponding box with the URL you copied
  * Click "Next"
* There shold now be a new entry called `CCI Platform`. Click the "Active" box next to that entry and click "Ok"

To format code at anytime, use either the "Ctrl+Alt+L" shortcut or navigate to _Code_ -> _Reformat Code_

### VS Code
* Click on the "Extensions" pane
* Search `checkstyle` and install the "Checkstyle for Java" plugin
* Pulling the checkstyle XML
  * In a browser navigate [here](https://github.com/philips-internal/cci-platform-checkstyle/blob/main/checkstyle.xml)
  * Click on the "Raw" button
  * Copy the link the address bar
  * Back in VS Code navigate to _File_ -> _Preferences_ -> _Settings_
  * Search `checkstyle`
  * In the setting titled "Java › Checkstyle: Configuration" paste in the URL you copied
