# VS Code Default Theme Override (OS: Windows)
Quick and easy way to override the default "Dark Plus (Default)" theme a in VS code with any theme you'd like without downloading one using the marketplace. Useful if you like a theme and don't want loose it due to a publisher deleting or updating it unfavourably.
<br><br>
1. VS Code themes are mostly just JSON files
2. First find a theme you like, my favourite is [Night Owl](https://github.com/sdras/night-owl-vscode-theme/) but you can find plenty on [Github](https://github.com/topics/vscode-theme). Just make sure to always look for the main [JSON File](https://github.com/sdras/night-owl-vscode-theme/blob/main/themes/Night%20Owl-color-theme-noitalic.json) which contains the theme information
3. With the JSON file open, use <kbd>Win</kbd> + <kbd>R</kbd> and navigate to ```%userprofile%\AppData\Local\Programs\Microsoft VS Code\resources\app\extensions\theme-defaults\themes``` and look for ```dark_plus.json``` which is the default VS code theme, open this file in VS code.
4. Then simply fold the ```"colors"``` and ```"tokenColors"``` arrys by hovering near the line number and clicking <kbd>></kbd>.
/
![image](https://user-images.githubusercontent.com/85340352/205795716-5561c10a-1d86-410e-bfac-d4eae7c2095b.png)

5. Finally copy & replace these (and all the nested code in between should also copy automatically) over from the theme into dark_plus.json. If ```"tokenColors"``` is missing in dark_plus just add it in underneath where ```"colors"``` ends.
6. Press save and it's done. Simply reload VS code and your theme is now embedded directly into VS code.

## Extra tips
1. When you are done, go back to ```%userprofile%\AppData\Local\Programs\Microsoft VS Code\resources\app\extensions\theme-defaults\themes``` and make a copy of dark_plus.json. Then when installing VS Code on a new machine, all you need to do is navigate to the same folder and replace the original dark_plus.json with your own :)

2. To revert you can always visit the [Official dark_plus.json](https://github.com/microsoft/vscode/blob/main/extensions/theme-defaults/themes/dark_plus.json) repository and download the original version should you want to go back.

3. You can skip all the above (if you want the night owl theme) and just download the [modified JSON file](https://github.com/jaytabase/vscode_defaulttheme_override/blob/main/dark_plus.json).
