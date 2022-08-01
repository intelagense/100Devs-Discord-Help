# 100Devs-Discord-Markdown
Unsanctioned supplemental files and information for the 100Devs Discord.

## What is the purpose

Primarily created to collaborate on markdown examples for code snippets in pinned messages.
This README covers the use of Markdown. The channel directories include suggestions for pinned messages for specified Discord channels. 

## Markdown differences between Pandoc and Discord

In standard Pandoc Markdown you can demonstrate to viewers how code blocks are created by nesting a triple-backticked code block within a quadruple-backbacked code block

<!--- Note: If you are viewing this file in raw mode please realize that I am using an additional layer of codeblocks in order for GitHub to create this README--->
`````
````
```[language]
  [code]
```
````
`````

Discord Markdown requires that you insert a Zero Width Space (U+200B) within any triple-backticks you wish to escape
````
```             //normal triple-backtick
`​``[language]   //escaped triple-backtick (No visible difference due to the Zero Width Space.)
  [code] 
`​``
```
````

## Applying syntax highlighting 
When specifying the [language] in a code block Discord will normally apply syntax highlighting. This highlighting is lost when using nested code blocks. You can manually apply syntax highlighting in your code block using ANSI syntax in your markdown.

<p>This code...</p>

````
```ansi
`​``[34mjavascript[0m
[32mconst[0m markdown = tricky;
[32mif[0m([36m'difficult'[0m){
  [31mconsole[0m.log([36m'copy + paste'[0m)
}
`​``
```
````

<p>which looks like this when editing in Discord...</p>
<img src="images/discordansi.png">
<p>will display as this to other users.</p>
<img src="images/discordansirender.png">
<p>Using ansi color in examples will help the viewer to understand why the [language] is included after the triple-backticks.</p>

*Alternately you could just include a screenshot every time, but that seems very wasteful.*
