# micahs-vscode-guide
My guide on maximizing efficiency with my favorite code editor –  VSCode

### Finding the Right Theme
I personally use the [**Palenight Theme**](https://marketplace.visualstudio.com/items?itemName=whizkydee.material-palenight-theme)
- Change the theme and browse themes by opening the command pallette (Command + Shift + P) and typing `Preferences: Color Theme`

### Extensions!!!
I use a lot of extensions. I currently have 91 installed, but I will go over some of my favorites and rank them in this guide.

1. [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) Automatically rename paired HTML/XML tag. This is particularlly useful for my React projects.
2. [Camel Case](https://marketplace.visualstudio.com/items?itemName=MarioQueiros.CamelCase) Will Transform selected text in camel case notation. Very useful when having a lot of cursors at the same time
3. [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) This is great for spell checking variable names and comments. It will even be able to spellcheck camelCase.
4. [Color Picker](https://marketplace.visualstudio.com/items?itemName=anseki.vscode-color&ssr=false#review-details) This is great to see the color of a hex value and change it easily. 

![Demonstration of Color Picker](https://raw.githubusercontent.com/anseki/vscode-color/master/s-01.gif)

5. [DotEnv](https://marketplace.visualstudio.com/items?itemName=mikestead.dotenv) This is great for handling .env files and coloring them correctly 

![Demonstration of DotEnv](https://raw.githubusercontent.com/mikestead/vscode-dotenv/master/images/screenshot.png)

6. [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens) A great Extension to view Git commits, branches, stashes, and to be able to see who wrote each line of code, and when they wrote it

![Demonstration of GitLens](https://raw.githubusercontent.com/gitkraken/vscode-gitlens/main/images/docs/commits-view.png)

7. [Increment Selection](https://marketplace.visualstudio.com/items?itemName=albymor.increment-selection) This will allow incrementing or decrementing numbers using multiple cursors (very useful)

![Demonstration of Increment Selection](https://github.com/albymor/Increment-Selection/raw/master/images/demo.gif)

8. [Multi Cursor Case Preserve](https://marketplace.visualstudio.com/items?itemName=Cardinal90.multi-cursor-case-preserve) This will preserve case when using multiple cursors. One of my most useful extensions

![Demonstration for Case Preserve](https://github.com/Cardinal90/multi-cursor-case-preserve/raw/master/images/Example.gif)

9. [Node Readme](https://marketplace.visualstudio.com/items?itemName=bengreenier.vscode-node-readme) This will allow you to view the npm documentation on a package in the editor

![Demonstration of Node Readme](https://raw.githubusercontent.com/bengreenier/vscode-node-readme/master/images/example-import.gif)

10. [Prettier Code Formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) This is my code formatter of choice. I have VSCode format on save so I use this a lot
11. [Project Manager](https://marketplace.visualstudio.com/items?itemName=alefragnani.project-manager) This is very nice when you have a lot of projects. It will show up as a different tab on the left panel and will allow you to easily swap between projects

![Demonstration of Project Manager](https://raw.githubusercontent.com/alefragnani/vscode-project-manager/4e8b7ddf030ed005aaca9393c67f28d7ca9f4b19/images/vscode-project-manager-side-bar-tags.gif)

12. [Remote SSH](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh) An amazing package that will ssh you into a machine and the entire VSCode editor will be at your disposal. No need for scp or vi. You can code directly in VSCode on the machine

13. [Selected Character Count](https://marketplace.visualstudio.com/items?itemName=mousetraps.selected-character-count) This is very useful. If you want to know how many zeroes there are in a string, how many characters, etc. Just highlight the text and do "Character Count" in the command 

![Demo for Character Count](https://user-images.githubusercontent.com/762848/36338135-07014900-135c-11e8-80e3-ec2a24501d85.png)

14. [Tabnine AI Autocomplete](https://marketplace.visualstudio.com/items?itemName=TabNine.tabnine-vscode) This is similar to GitHub copilot, and it will give some very helpful autocomplete coding suggestions

![Demo for Tabnine](https://github.com/codota/TabNine/raw/master/with-and-without-tabnine-java.gif)

15. [Turbo Console Log](https://marketplace.visualstudio.com/items?itemName=ChakrounAnas.turbo-console-log)

![Demo for Turbo](https://image.ibb.co/dysw7p/insert_log_message.gif)

16. [TypeScript Importer](https://marketplace.visualstudio.com/items?itemName=pmneo.tsimporter) Automatically searches for TypeScript definitions in workspace files and provides all known symbols as completion item to allow code completion.

![Demo for Typescript importer](https://raw.githubusercontent.com/pmneo/ts-importer/master/demo.gif)

### VSCode Preferences
1. Enable Bracket pair colorization `Editor › Bracket Pair Colorization: Enabled`
2. Change `Editor: Multi Cursor Modifier` to `ctrlCmd` which will allow you to hold command on mac and click to add more cursors

### Keyboard Shortcuts (can set in Preferences > Keyboard Shortcuts)
- For previous Atom users: Use the [Atom Keymap Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode.atom-keybindings) and the keybindings should be familiar
- `Command + Shift + P` will be defaulted to open the command palette
- `Command + Shfit + L` should be set to `Search Editor: Select All Matches` - this is very useful. When you search for text, you can do this keybinding and press `esc` and cursors will be put at each occurrence of the text. This is more powerful than the basic `Find and Replace`. You can add entire sections of code or edit things other than the common occurrance as well.
- `Command + J` should be set to `View: Toggle Panel Visibility` - this will hide and close the terminal easily
- `Command + Shift + D` should be set to `Copy Line Down` - this is how to duplicate lines or selections
- `Option + DownArrow` should be set to `Move Line Down` and `Option + UpArrow` should be set to `Move Line Up`
- `Control + K` should be set to `Delete All Right` - this will delete an entire line of code
- `Control + Command + DownArrow` should be set to `Add Cursor Below` and `Control + Command + UpArrow` should be set to `Add Cursor Above`
- `Command + \` should be set to `View: Toggle Primary Side Bar Visibility` - this will toggle hiding the left sidebar that contains the explorer. Useful for when in small windows

### Advanced Guide for Multiple Cursors
Being able to change an entire csv file to a json file all at once with multiple cursors is very powerful. I try to use multiple cursors as much as possible, but there is a learning curve to how to do it correctly. Just like `Replace all`, you must be careful when using a lot of cursors at once.
1. There are multiple ways to add cursors
  - Holding `Control` and clicking the cursor on where you want the cursor (Make sure to set the preference in the VSCode Preferences section)
  - Using the keybinding you set earlier `Control + Command + DownArrow` or `Control + Command + UpArrow`
  - Using the keybinding you set earlier `Command + Shfit + L` after searching for occurrances of text to add a cursor at each occurrance
  - Pro Tip: You can hold `Command` and click on a cursor to remove it
2. After adding your cursors, you must make sure to follow the pattern of each line. Look at this example below:
```
const x = 2000;
...
const exampleVar = 2;

```

- To change both value to have a string value of `"samplestring"`, you would first add a cursor to each line. Use a method above, I would recommend starting with just doing `Command` and clicking somewhere on each line. 
- I like to put the cursor on a random place on each line and then do `Command + LeftArrow` to go to the beginning of the line. This way both cursors are at the same place.
- Then you will notice some differences in each line. If you simply use the arrow keys to navigate, variables `x` and `exampleVar` will mess up your cursor alignment since they have a different amount of characters. Instead, navigate while holding `Option` and the arrow keys. This will move your cursors by each word instead of each character
- Now move your cursors to the beginning of each value. 
