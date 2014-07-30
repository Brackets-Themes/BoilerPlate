BoilerPlate
===========

This is a boilerplate project to get you started with the essentials to create your new theme as an extension.  Clone this repo and start customizing your theme by modifying main.less.

In order to install your new theme, you need to publish it to a git repo and install it via the extension manager.

### How do you manually install a Theme? ###

We will use this boilerplate to illustrate a simple workflow.

1. Install the boilerplate theme by going through Brackets extension manager and install it using the URL `https://github.com/Brackets-Themes/BoilerPlate`.
  1. Or you can bundle it up as a zip and drag the zip into the extension manager.
1. Select the Brackets View menu and click Themes…
1. Choose "Title for my theme" to select the boilerplate as the theme.
1. That's it!

### Customizing BoilerPlate ###

Now that you have installed and selected boilerplate theme, you can customize it.  Since the theme was installed as an extension, you will need to navigate to the extensions folder to get to the theme.  Go ahead and do that and open main.less, and start adding your favorite colors.  Notice that when you make changes to main.less, the changes will automatically be applied when you save those changes. I personally do all my customization to main.less right from Brackets so that I can see my changes right as I work.

### Important bits of a Theme extension ###

1. The most important bit, the theme file.  This can be a css or a less file with all your css rules.  This is the file you modify when you want to make your own custom theme.  In boilerplate, it is `main.less`.
2. It needs a `package.json`, the same way all other Brackets extensions need one.
3. The `package.json` must have a `theme` object.  This object as of right now contains a `file` field, which is the file name; in the case of BoilerPlate, it is "main.less".  Another field is `dark`, which is a boolean that tells Brackets to setup an all around dark theme.
4. It must have a `name` field, with the name for the theme. In BoilerPlate the name is simply "boilerplate".
5. For now, your theme extension needs to have a main.js, as that is a requirement for extensions to be installed.  The file should be completely empty.
