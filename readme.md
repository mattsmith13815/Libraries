## NPM Libraries
## add new library, to make available for local projects using npm
- npm install {package} -- prefix npm/{package}
- example: npm install lodash --prefix npm/lodash

## setup local npm to use private repo
Method 1: Configure npm Globally
- Create or Edit the .npmrc File:
- On Linux and macOS, create or edit the file ~/.npmrc.
- On Windows, create or edit the file %USERPROFILE%\.npmrc.
- Add the Private Repository URL:
- registry=https://your-private-repo-url/

Method 2: Configure npm for a Specific Project
- Create a .npmrc File in the Project Directory:
- Create a file named .npmrc in the root directory of your project.
- Add the Private Repository URL:
- Add the following line to the .npmrc file:
- registry=https://your-private-repo-url/

## Python Libraries
## add a new library, to make available for Python:
- pip install requests --target requests

## setup local pip to use private repo
- create a file: pip.conf:

- On Linux and macOS, create or edit the file ~/.pip/pip.conf.
- On Windows, create or edit the file %APPDATA%\pip\pip.ini.
- or
- Create a file named pip.conf in the project directory.

pip.conf contents:
[global]
extra-index-url = https://your-private-repo-url/