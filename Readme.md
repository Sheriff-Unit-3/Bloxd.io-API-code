# Readme
> [!NOTE]
> This file doesn't include documentation for Bloxd.io coding, but instead is to serve as a resource for understanding Bloxd.io code and how to it works.

## About this repository
This was created because the original documentation was not well explained or organized in any way and lacked information that many people agreed would be helpful. So here it is, it not perfect, but it contains more information then the original documentation. There may from time to time be errors in the documenation and it may lack newer information. That's why it's highly recomended that if you notice that there's missing information or that there's an error somewhere that you create a pull request. Also if you think that you have information that may be helpful to new coder that you create a pull request to add it here under the `Information` header. You will find that most of the files here are not formated the same as the original documentation, this is on purpose so that it's easier to search through for the information you want.

## Information
> [!NOTE]
> This section needs information, please create a pull request if you have information for this section.

## FAQ
**Q:** What is the `playerId` in functions and callbacks?  
**A:** It is field that contains the Id of a player. In `Code Blocks` and `Press to Code` signs it can contain the varible `myId` which will return the Id of the player that activated the code. In `World Code` though `myId` doesn't work cause code gets activated by callbacks. So instead in the `playerId` field in the callback we can place somthing like `pId` and that will define `pId` as the playerId of the player that triggered that callback. So we would can then place `pId` in to the `playerId` field in functions in that callback.  

**Q:** Where can I use callbacks?  
**A:** You can only use callbacks in `World Code` cause `Code Blocks` and `Press to Code` signs only get activated when a player presses them.

**Q:** What is the difference between `World Code` and `Code Blocks`?  
**A:** `World Code` runs all the time and when a callback in `World Code` get triggered it runs the code in that callback. `Code Blocks` though only get triggered when a player presses them or a sign next to them gets triggered. But `World Code` is limited to 16,000 characters (including spaces) and you can only have one `World Code` for each world. But even though `Code Blocks` are also limited to 16,000 characters as well, you can have an unlimited amount of them.
