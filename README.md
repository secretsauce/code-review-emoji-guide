# 📘 Code Review Emoji Guide

A simple emoji legend to help succinctly convey added meaning in code review comments.

> ~~A picture is worth 1,000 words.~~ _An emoji is worth 20 words._

A little bit of emoji can go a long way when it comes to code reviews and make giving and receiving code review a little bit more enjoyable 😃.

Using CREG (Code Review Emoji Guide) puts a little bit more ownership on the reviewer to give the reviewee added context and clarity to follow up on code review. For example, knowing whether something really requires action (🔧), highlighting nit-picky comments (⛏), and clarifying items that don’t necessarily require action but are worth saying ( 📝, 🤔, 🌵, 💯)

## Emoji Legend

|     |   `:code:`   | Meaning                                                                                                                                                                             |
| :-: | :----------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 👏 <br/> or <br/>💯 | `:clap:`<br/> or <br/>`:100:`  | I like this... <br /><br /> ...and I want the author to know it! This is a way to highlight positive parts of a code review.                                                        |
| 🔧  |  `:wrench:`  | I think this needs to be changed. <br /><br />This is a concern or suggested change/refactor that I feel is worth addressing.                                                       |
| ❓ | `:question:` | I have a question. <br /><br /> This should be a fully formed question with sufficient information and context that requires a response.                                            |
| 🤔  | `:thinking:` | Let me think out loud here for a minute. <br /><br /> I might express concern, suggest an alternative solution, or walk through the code in my own words to make sure I understand. |
| 📝  |   `:memo:`   | This is an explanatory note, fun fact, or relevant commentary that does not require any action.                                                                                     |
| ⛏   |   `:pick:`   | This is a nitpick. <br /><br /> This is likely fine as-is and may include insignificant refactor suggestions, code formatting, etc...                                               |
| 🏕  | `:camping:`  | Here is an opportunity, ( may or may not be directly related to your changes) for us to _leave the code cleaner than we found it_ ([boy scout rule](http://www.informit.com/articles/article.aspx?p=1235624&seqNum=6)).                                      |
| 📌  | `:pushpin:`  | This is a concern that is _out of scope_ and should be staged appropriately for follow up.                                                                                          |
| 🌵 | `:cactus:`  | The code here can be `DRY`'ed (Don't Repeat Yourself), it could be as simple as putting computed values on a constant or abstracting this into a function.   |
| 💧 | `:droplet:`  | The opposite of `DRY`. `WET` (Write Everything Twice), sometimes fancy abstractions can obfuscate the code and make it hard to understand or refactor. Consider repeating/spelling out some or all of the logic instead. (_see_ [single responsibility principle](https://en.wikipedia.org/wiki/Single_responsibility_principle))  |
| 🚚  | `:truck:`  | The naming of this statement (ie. const, var, function, etc.) is not declarative and needs to be renamed (moved). Try to be clear about what this is doing, avoid using acronyms or short names. |
| 👾  | `:space_invader:` | The formatting of the code has either too little or too many spaces (or blank lines) and makes it hard to read. |
| ✅ | `:white_check_mark:` | This needs tests. Enough said. |
| 🌅 | `:sunrise:` | Return early, use [guard clauses](https://refactoring.com/catalog/replaceNestedConditionalWithGuardClauses.html). [Exiting early allows you to pop stuff off your limited mental stack.](https://softwareengineering.stackexchange.com/questions/18454/should-i-return-from-a-function-early-or-use-an-if-statement#comment27703_18459)  |


## Usage

Prepend comments with the appropriate emoji to convey the meaning associated with it, or just add the emoji and point them to this guide.

## Examples:

```
 🔧  - We do have an existing module, `great-module.js`, that accomplishes this same task. Let's pull it in and replace your implementation with it.
```
```
 ⛏  This if statements could be simplified down to a single ternary expression.
```

```
  💯 , Wow, nice refactor. Thanks for fixing this up.
```
```
 📌  We really need to invest some time in refactoring out our use of this deprecated library. _Issue created: [LINK TO ISSUE]_.
```
```
 🚚  :  this function could be renamed from `getAccUsrs` to `getAccountUsers` for clarity.
```
---

### Credits

Partially inspired by

* https://github.com/erikthedeveloper/code-review-emoji-guide
* http://dawehner.github.io/github,/code/review/2017/09/08/emoji-code-review.html
* https://gist.github.com/pfleidi/4422a5cac5b04550f714f1f886d2feea
* https://twitter.com/JackieCalaprist/status/981557821308153856
* https://github.com/carloscuesta/gitmoji/
