# cci-platform-common

## Checkstyle
### Local Setup

#### Intellij
* Navigate to _File_ -> _Settings_ -> _Plugins_, search `checkstyle` and install the "Checkstyle-IDEA" plugin
* Navigate to _File_ -> _Settings_ -> _Tools_ -> _Checkstyle_
* In the _Configuration File_ section, click on the "+"
* For _Description_ type `CCI Platform`
* Underneath the "Use a local Checkstyle file", use the file browser to select the `checkstyle.xml` file in the `.cci-common` folder of your repo
* Click "Next"
* There shold now be a new entry called `CCI Platform`. Click the "Active" box next to that entry and click "Ok"

To format code at anytime, use either the "Ctrl+Alt+L" shortcut or navigate to _Code_ -> _Reformat Code_

#### VS Code
* Click on the "Extensions" pane
* Search `checkstyle` and install the "Checkstyle for Java" plugin
* Navigate to the `.cci-common` folder
* Right click on the `checkstyle.xml` and click the "Set the Checkstyle Configuration file" option

#### Command Line
All configurations are already included in CCI Common. Run `./gradlew checks` to execute all checkstyle tasks

## Updating the CCI Common submodule
If you're noticing that your builds are failing due to checkstyle warnings but none are popping up locally, it's most likely the case that this repository has been updated and the one you're working on hasn't pulled those changes yet. Simply navigate to the `.cci-common` folder in your repository via a command line and run `git pull`. Then add/commit/push the changes to your remote branch.
