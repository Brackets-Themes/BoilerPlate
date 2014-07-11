BoilerPlate
===========

This is a boilerplate project to get you started with the essentials to create your new theme as an extension.  Clone this repo and start customizing your theme by modifying main.less.<br>

In order to install your new theme, you need to publish it to a git repo and install it via the extension manager.  But before you can do all that, you need to setup your environment.  ThemesManager will soon ship with Brackets so you will not have to setup a dev environment.

### Setting up your dev environment ###

1. Install the latest Brackets build (this gives you the native shell binaries which you'll use in step 4)
2. Fork the [brackets repo](https://github.com/MiguelCastillo/brackets/tree/themes-v1) `git clone https://github.com/MiguelCastillo/brackets.git -b themes-v1 /bracketsThemes`
3. Fetch submodules: `cd bracketsThemes` and `git submodule update --init`
4. Run `setup_for_hacking` script:

    |  |  |
    |---|---|
    | Mac | `tools/setup_for_hacking.sh "/Applications/Brackets.app"` |
    | Windows | `tools\setup_for_hacking.bat "C:\Program Files (x86)\Brackets"` <br>_(MUST be run in a Command Prompt started with "Run as Administrator")_ |
    | Linux | `sudo tools/setup_for_hacking.sh "/opt/brackets"` |

Now, when you launch the Brackets app it will load your git copy of the source code, rather than the original source code that was distributed with the installer.


### How do you install a Theme? ###

We will use this boilerplate to illustrate a simple workflow.<br>

Once Brackets is setup for hacking, install the boilerplate theme by going through Brackets extension manager and install it using the URL <code>https://github.com/Brackets-Themes/BoilerPlate</code>.

### Selecting a Themes? ###

From the View menu, select Themes menu to present you with a dialog where you can chose your themes from.  Choose "Title for my theme" to select the boilerplate as the theme.  That's it!

### Customizing BoilerPlate ###

Now that you have installed and selected boilerplate theme, you can customize it.  Since the theme was installed as an extension, you will need to navigate to the extensions folder to get to the theme.  Go ahead and do that and open main.less, and start adding your favorite colors.  Notice that when you make changes to main.less, the changes will automatically be applied when you save those changes. I personally do all my customization to main.less right from Brackets so that I can see my changes right as I work.

### Important bits of a Theme extension ###

1. The more important bit, the theme file.  This can be a css or a less file with all you css rules.  This is the file you modify when you want to make your own custom theme.  In boilerplate, it is main.less.
2. It needs a package.json, the same way all other Brackets extensions need one.
3. The package.json must have a <code>theme</code> field.  This is the name of the theme file to be loaded. In the boilerplate project, it is called main.less so ThemeManager will load main.less.
4. It must have a <code>name</code> field, with the name for the theme.  In BoilerPlate the name is simply "boilerplate".
5. For now, your theme extension needs to have a main.js, as that is a requirement for extensions to be installed.  It can be empty.
 
