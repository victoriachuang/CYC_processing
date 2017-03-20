# CYC_processing
A processing guide for the Gatehouse Media community content team with shortcuts and hotkeys

## GREP find-and-replace

The GREP find-and-replace tab in InCopy allows you to search for patterns in the text, rather than search-term matches alone. This is especially helpful when you’re looking for things that occur in a certain position (beginning of a line, end of line) or when you don’t know the exact search term (two or more spaces). However, because some of these characters are “reserved” for certain patterns, you should be careful when using GREP to find and replace text with special characters, such as periods, dollar signs and backslashes. Before tackling your brief in InCopy, you can make sure your regular expression works at [rubular.com](http://rubular.com/).

|Function|Find what|Change to|Notes|
|--------|---------|---------|-----|
|Turn "n" into bullet point|`^n`|`~8`||
|Get rid of extra whitespace|`(\s){2,}`|`\s`||
|Remove space from the beginning of a line|`^(\s)`|`# leave blank`||
|Remove space from the end of a line|`(\s)$`|`# leave blank`||
|Cable schedules with dates formatted like "Ipswich Board of Selectmen Meeting Live 12/7/15"; change date to Dec. 7, 2015|`(\s12\/)` then `(\/15)$`|`Dec.` then `.2015`||
|Turn returns into whitespace|`\r`|`\s`|Note that this will change **every** return into a space, ie. turning your brief into one long paragraph, so you might want to make a more unique identifier. You can also append `\s` with things you want to join each line with, such as semicolons, commas, etc.

## General keyboard shortcuts for OSX

You'll love not having to find your cursor.

### Text keyboard shortcuts
|Function|Shortcut|
|--------|--------|
|Jump to beginning of line|`Control` + `A`|
|Jump to end of line|`Control` + `E`|
|Remove formatting|`Command` + `\`|

### Application shortcuts
|Function|Shortcut|Notes|
|--------|--------|-----|
|Switch between applications|`Command` + `Tab`||
|Switch between windows of the same application|`Command` + `~` (the key above tab)||
|Screen shot|`Command` + `Shift` + `3`|Will save to desktop|

### Chrome keyboard shortcuts
|Function|Shortcut|Notes|
|--------|--------|-----|
|Close current tab|`Command` + `W`||
|Close window|`Command` + `Shift` + `W`||
|Switch between tabs|`Command` + `Option` + right or left arrows|If you have [Spectacle](https://www.spectacleapp.com/) installed, the Spectacle shortcuts will override this.|
|Jump to first tab|`Command` + `1`|Replace 1 with any digit for the `n`th tab|
