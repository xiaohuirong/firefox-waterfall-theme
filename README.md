<div align="center">

<h1><pre>+-----+-----+-----+-----+-----+-----+-----+
| █▀▀ | ▄▀█ | █▀▀ | █▀▀ | ▄▀█ | █▀▄ | █▀▀ |
| █▄▄ | █▀█ | ▄▄█ | █▄▄ | █▀█ | █▄▀ | ██▄ |
+-----+-----+-----+-----+-----+-----+-----+</pre></h1>

![Preview Image showing both the one-line style and the style for smaller screensizes.](assets/preview.png)

</div>          

Cascade, Mouse Edition, is a Firefox Style based on the Cascade theme by Andreas Grafen.
What you get is a really simple one-line layout using the new Proton UI.
          
Some minor tweaks includes :
- tab close button on hover
- window control buttons
- hamburger menu button
- color changes for added contrast
- inactive & active tab size
          
The original Cascade Theme by Andreas Grafen was based on SimpleFox :
      > SimpleFox: https://github.com/migueravila/SimpleFox

                  
Authors:       
- Andreas Grafen (original cascade theme) (https://andreas.grafen.info)
- Clément Rambaud (minor tweaks on the original file for a more mouse-centered use)

On larger window resolutions Cascade will have a oneline layout which displays the URL bar and tab list next to each other. Smaller resultions will stack both UI elements on top of each other for better readability.

Thank you [Nick](https://github.com/nicksundermeyer) for all the great suggestions for improvements! ♡

‎
‎
‎
‎
‎

## Contents
- [Installation](#how-to-use-a-userchromecss-theme)
- [Customisation](#customise-cascade-to-your-liking)
- [Keyboard Shortcuts](#keyboard-shortcuts)

‎
‎
‎
‎
‎

## How to use a userChrome.css theme

1. Type `about:config` into your URL bar. Click on the **I accept the risk** button if you're shown a warning.
2. Seach for **`toolkit.legacyUserProfileCustomizations.stylesheets`**, **`layers.acceleration.force-enabled`**, **`gfx.webrender.all`** and **`svg.context-properties.content.enabled`** and set them to **`true`**.
3. Go to your profile folder:
    - Linux: `$HOME/.mozilla/firefox/######.default-release/`
    - MacOS: `Users/[USERNAME]/Library/Application Support/Firefox/Profiles/######.default-release`
    - Windows: `C:\Users\[USERNAME]\AppData\Roaming\Mozilla\Firefox\Profiles\######.default-release`
4. If it doesn't exist already create a folder called `chrome`.
5. Copy your desired `userChrome.css` into that folder.
6. *optional* Customise everything to your liking.

‎
‎
‎
‎
‎

## Customise Cascade to your liking

‎
### Breakpoint

Edit the `min-width` value to change the breakpoint size on which Cascade will switch to the oneline layout.

```css
@media (min-width: 1000px) {
    
    [...]
    
}
```

‎
### Colours

You can use your own colours for Cascade. To do so just edit the following block on top of the config section.
By default it will use a dark theme but colour suggestions for light theme users are given as well. Please also change Firefox' theme in your settings to make sure you get the best compatibility.

If you're using a custom colour scheme (e.g. [Firefox Color](https://color.firefox.com)) you can comment out the entire block to use the default colours provided by the Theme Addon.

```css
 :root {
    
    /* main window colour – toolbar & window background */
    --window-colour:    #1E2021;

    /* accent colour – active tab, button hover, ... */
    --secondary-colour: #191B1C;

    /* text and highlight colour */
    --inverted-colour:  #FAFAFC;

}
```

‎
‎
‎
‎
‎

## Keyboard Shortcuts

This userstyle was made for a keyboard centered usage, like Tilling Window Manager users or just cool people that loves them!
These are **some** of the shortcuts that are available:

Windows / Linux | MacOS | Description
--- | --- | ---
`Ctrl + L` | `Command * L` | focuses the URL bar
`Ctrl + B` | `Command + B` | shows you the bookmark sidebar
`Ctrl + Shift + B` | `Command + Shift + B` | shows you the bookmark toolbar
`Alt + Left Arrow` | `Command + Left Arrow` | navigates backwards in your history
`Alt + Right Arrow` | `Command + Right Arrow` | navigates forwards in your history
`Ctrl + T` | `Command + T` | opens a new tab
`Ctrl + Shift + T` | `Command + Shift + T` | reopens the last closed tab
`Ctrl + W` | `Command + W` | closes the current tab
`Ctrl + Page Up`<br/>or `Ctrl + Shift + Tab` | `Command + Option + Left Arrow` | navigates to the previous tab
`Ctrl + Page Down`<br/>or `Ctrl + Tab` | `Command + Option + Right Arrow` | navigates to the next tab

For the full list of shortcuts visit [the official Firefox website](https://support.mozilla.org/en-US/kb/keyboard-shortcuts-perform-firefox-tasks-quickly).‎
‎
‎
‎
‎
