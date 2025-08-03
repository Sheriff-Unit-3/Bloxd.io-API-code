# Readme
> [!NOTE]
> This is not the official documentation and is not edited or run by any of Bloxd.io's Devs, this is ment to be an additional resource to the official documentatio.
> [!WARNING]
> This repository may contain out-of-date or incorrect information at times, but the maintaners will try to keep this as up-to-date and correct as they can.
> [!TIP]
> Find information that you think should be added or changed? Create a pull request!

You can run javascript when right clicking code blocks and press to code boards.
This is only available to owners of worlds lobbies.
The javascript can interact with the Bloxd.io game api.

Please use [Bloxd.io's official discord server](https://discord.gg/vwMp5y25RX) to report any issues you come across or features you'd like to see added.
Please create a pull request if you notice incorrect, or missing information in this version of the documenation.

## Code Blocks

- World owners can find these by searching in the creative menu
- No need to add `press to code`, this text is only needed for code boards, and will automatically be removed
- If you want to run code without opening the code editor, you can trigger the code block by right clicking an adjacent `press to code` board instead

## Boards

- You can begin a board with `press to code` to run javascript when you right click it.
- Normally you can't edit a code board after placing it, but you can currently work around this by putting a space before `press to code`.
- Boards only allow for a small amount of text, we recommend you use Code Blocks instead, or you can work around this by using multiple boards

## Notes

- Global variable `myId` stores the player ID of who is running the code, it can not be used in World code.
- Global variable `thisPos` stores the position of the currently executing code block or press to code board, it can not be used in World code.
- You can use `api.log` or `console.log` for printing and debugging (they do the same thing).
- You can use `Date.now()` instead of `api.now()` if you prefer, both return the time in milliseconds.
- Comments like `/* comment */` work.

> [!NOTE]
> The official documentation will say that `// comments` will not work, but that is incorrect as they now work.
  
## About this repository
This was created because the original documentation was not well explained or organized and lacked information that many people agreed would be helpful. So here it is, it's not perfect, but it contains more information then the original documentation. There may from time to time be errors in the documenation and it may lack newer information. That's why it's highly recomended that if you notice that there's missing information or that there's an error somewhere that you create a pull request. Also if you think that you have information that may be helpful to new coder that you create a pull request to add it here under the `Information` header. You will find that most of the files here are not formated the same as the original documentation, this is on purpose so that it's easier to search through for the information you want.

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
