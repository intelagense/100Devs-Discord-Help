# 100Devs-Discord-Markdown
Unsanctioned supplemental files and information for the 100Devs Discord.

## What is the purpose

Primarily created to collaborate on markdown examples for code snippets in pinned messages.

In Pandoc Markdown you can demonstrate how to create code blocks by nesting a triple-backticked code block within a quadruple-backbacked code block

<!--- Note: If you are viewing this file in raw mode please realize that I am using an additional layer of codeblocks in order for GitHub to create this README--->
`````
````
```[language]
  [code]
```
````
`````

In Discord Markdown you must use insert a Zero Width Space (U+200B) within the triple-backticks you wish to escape
````
```             //normal triple-backtick
`​``[language]  //escaped triple-backtick
  [code] 
`​``
```
````

In order to display syntax highlighting you must go even one step further using ANSI syntax in your markdown.

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
