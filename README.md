# Redmond-Firefox
A collection of Internet Explorer inspired themes for Firefox
![Image Screenshot](https://github.com/matthewmx86/Redmond-Firefox/blob/master/Screenshots/Screenshot1.png)
## About
The Redmond-Firefox project aims to create a Firefox theme mimicking classic Internext Explorer 6 and 8 styles.
The project originally started when I was designing Firefox themes to go along with my GTK Redmond97 and Redmond2K themes.

## Requirements
#### Main theme
The following are required:
```
firefox
```

## Limitations
Inherit color support is not currently finished.
Also the theme was designed with a certain color scheme in mind so it may not display correctly
with certain color schemes. I'm working on adding inherit functions to the theme and I'm currently 
designing a script to apply selected colors from the active GTK theme and apply it to the Firefox theme. 
For now I recommend using my default [Redmond97](https://github.com/matthewmx86/Redmond97) theme.

## Installation

There are two ways to get the theme source files. For convenience I always make a tar package of the repository after any updates so you can download
the archive instead of cloning the whole repository for every update. You can find the archives [here](https://github.com/matthewmx86/Redmond-Firefox/tree/master/Packages).
For those who prefer to clone the repository you can download a copy of the repository by the following command:

```
git clone https://github.com/matthewmx86/Redmond-Firefox.git
```

To install, you will first need to find your firefox user profile directory. It is usually the one that ends with ".default".
To find the correct directory, open a terminal and go to the hidden Firefox directory. Using grep you can view the directories
ending with ".default".
```
cd ~/.mozilla/firefox
ls | grep default
```
In this exmaple I have two directories: one .default and the other .default-release. 
![Image Screenshot](https://github.com/matthewmx86/Redmond97/blob/master/Screenshots/console.png)
If you only have one directory ending with .default that one is the correct profile directory and you can skip
this next step. Otherwise, you can run the following to see which profile is the default.
```
firefox -P
```
You will then see the following window:

![Image Screenshot](https://github.com/matthewmx86/Redmond97/blob/master/Screenshots/firefox.png)

The selected profile is your default profile, in my case it is the default-release profile.

Once you have found the correct profile directory, you will then need to make a directory inside of it called "chrome".
Following my example above you would run the command:
```
mkdir ~/.mozilla/firefox/vugvl4ul.default-release/chrome
```
Now that the chrome directory has been created, you can install the theme by copying the contents of the repository/Firefox-userchrome directory or extracting the 
archive into your chrome folder. Again, using my example above the command would be:
```
cp -aR ~/Redmond-Firefox/Firefox-userchrome/* ~/.mozilla/firefox/vugvl4ul.default-release/chrome/
```
or from an archive:
```
tar -xvzf firefox_IE.tar.gz -C ~/.mozilla/firefox/vugvl4ul.default-release/chrome/
```

Note:
[ If you have not enabled custom user style sheets (userchrome): ]
1. Navigate to "about:config" in Firefox
2. Enter the following text in the search box: toolkit.legacyUserProfileCustomizations.stylesheets
3. Set the option toolkit.legacyUserProfileCustomizations.stylesheets to True
4. Close all instances of Firefox and the changes will take effect when you restart Firefox

The Firefox theme should now be installed and will be activated once you close all Firefox sessions and restart Firefox.

##Screenshots
![Image Screenshot](https://github.com/matthewmx86/Redmond-Firefox/blob/master/Screenshots/Screenshot1.png)
![Image Screenshot](https://github.com/matthewmx86/Redmond-Firefox/blob/master/Screenshots/Screenshot2.png)
![Image Screenshot](https://github.com/matthewmx86/Redmond-Firefox/blob/master/Screenshots/screenshot3.png)
![Image Screenshot](https://github.com/matthewmx86/Redmond-Firefox/blob/master/Screenshots/screenshot4.png)
![Image Screenshot](https://github.com/matthewmx86/Redmond-Firefox/blob/master/Screenshots/screenshot5.png)
