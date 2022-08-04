# 100Devs-Discord-Help `(Work in progress)`

Unsanctioned supplemental files and information for the 100Devs Discord help channels.

## Table of contents

**Getting started - asking questions in the Discord**
  * [How do I ask my question?](#how-do-i-ask-my-question)
  * Searching for previous answers.
  * Best time to ask?
  * [What about voice chat?](#what-about-voice-chat)
  * [What are code blocks?](#what-are-code-blocks)


[Frequently Asked Questions(coming soon!)](#)
  * How do I join catch-up crew?
  * What is a thread? and how does it work?
  
  
Answering questions
  * [How can I help?](#how-can-i-help)
  * [Code Blocks for 'pros'](#code-blocks-for-pros)

  
  


## Asking questions in the Discord

### How do I ask my question?

### Searching for previous answers.

### Best time to ask?

### What about voice chat?
Sometimes the fastest way to get your question answered is to join a voice chat and ask for help directly. You can also go into an empty voice chat and start sharing your screen and folx will show up out of curiosity. 

### What are code blocks?
One of Discord's features is that it uses 'Markdown' syntax to display text. You can surround the code you type in a chat with backticks and it will be displayed in a way that is easier for you and the other developers to read. 

Using three backticks in a row will create a multi-line code block. Type the name of the language you are using directly after the first triple-backtick to use syntax highlighting.

<img align="left" src="images/codesnip.png">

````
```[type the language here]
[paste your code here]
```
````

💡 Use single backticks to create an `` `inline code block` `` (Inline only, no color coding.)

## Frequently Asked Questions

### How do I join catch-up crew?

### What is a thread? and how does it work?
TLDR - A thread is basically a mini channel inside a main channel used to focus on a single topic. Messages sent inside the help channels are automatically transformed into a thread by the 'Needle Bot.'

💡 For more in-depth information on how Discord threads work check out the official [Discord threads FAQ (External link)](https://support.discord.com/hc/en-us/articles/4403205878423-Threads-FAQ)

## Answering questions

### How can I help?
>“If you have come here to help me, you are wasting your time. But if you have come because your liberation is bound up with mine, then let us work together.”<sub> -Lilla Watson</sub>

### Code blocks for 'pros'

Users not familiar with Markdown may be unaware that they can display their code using code blocks in Discord. 

In standard Pandoc Markdown you can show an example of how code blocks are created by nesting a regular triple-backticked code block within a quadruple-backbacked code block but this does not work in Discord.

<!--- Note: If you are viewing this file in raw mode please realize that I had to use yet another additional layer of codeblocks to create this README--->

`````
````
```[language]
[code]
```
````
`````

Markdown in Discord requires that you insert a Zero Width Space (U+200B) within any triple-backticks you wish to escape.
````
```             //normal triple-backtick
`​``[language]   //escaped triple-backtick (No visible difference due to the Zero Width Space.)
[code] 
`​``
```
````

#### Syntax highlighting hack

When specifying the [language] in a normal code block Discord will apply syntax highlighting. This highlighting is lost when using nested code blocks. You can manually apply syntax highlighting in your code block using ANSI syntax in your markdown. 

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
