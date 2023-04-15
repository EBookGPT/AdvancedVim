# Chapter 8: Navigating between Windows and Tabs in Vim

Welcome back! In the previous chapter, we covered Advanced Search and Replace Techniques in Vim, which can come in handy in various scenarios.

In this chapter, we will learn about navigating between windows and tabs in Vim. As you become more skilled in Vim, you will find that multiple windows and tabs are a useful way of working with multiple files at the same time.

Joining us as a special guest in this chapter is Drew Neil, an expert in Vim and author of [Practical Vim](https://pragprog.com/book/dnvim2/practical-vim-second-edition). His vast knowledge on the topic will help us explore the best practices to make navigation easier and more efficient.

We will cover several advanced techniques, including how to:

- Navigate between windows
- Move windows between tabs
- Create new tabs
- Switch between tabs

We will also delve into a few plugins that can enhance your experience navigating between windows and tabs, such as [vim-windowswap](https://github.com/wesQ3/vim-windowswap) and [vim-obsession](https://github.com/tpope/vim-obsession). 

Let's get started and take our Vim skills to the next level!
# Chapter 8: Navigating between Windows and Tabs in Vim - Exercise

Congratulations on making it this far! Now it's time to put your knowledge to the test with some hands-on practice. 

In this exercise, we will be working with multiple windows and tabs in Vim. This exercise assumes you already have a basic understanding of Vim and are comfortable working with multiple files in a single window.

## Exercise Overview

We will start by opening multiple files in Vim, creating new tabs and windows. Then we will use different techniques to navigate between them. Finally, we will close all the tabs and windows we opened during the exercise.

## Steps to Follow:

1. Open Vim and create a new file called `file1.txt`.
2. Type some random text in `file1.txt`
3. Open a new tab by typing `:tabnew` or `:tabe` and create a second file called `file2.txt`.
4. Type some text in `file2.txt` and save the file by typing `:w`.
5. Split the first window horizontally by typing `:split`.
6. Open a third file called `file3.txt`. Type some text in it and save it by typing `:w`.
7. Split the current window vertically by typing `:vsplit`.
8. Navigate between all the windows created by using various techniques such as `:wincmd h` for going to the left window, `:wincmd j` for going to the bottom window, and so on.
9. Test the plugin [vim-windowswap](https://github.com/wesQ3/vim-windowswap) by swapping the content between two windows, horizontally by typing `:WinSwap h` and vertically by typing `:WinSwap v`
10. Navigate between all the tabs created by typing `gt` to move to the next tab and `gT` to move to the previous tab.
11. Create a new tab and switch back to the previous tab. 
12. Save the current session by typing `:mksession vim-exercise.vim` and exit Vim by typing `:qa`. 
13. Open Vim again, and restore the previous session by typing `vim -S vim-exercise.vim`.


Great job! You have successfully practiced the techniques discussed in this chapter. Keep practicing, and you will become a Vim ninja in no time.
In this exercise, we used various Vim commands, techniques, and plugins to navigate between windows and tabs. 

Some of the commands we used are:

- `:tabnew` or `:tabe`: Creates a new tab in Vim
- `:split` or `:vsplit`: Splits the current window horizontally or vertically, respectively
- `:wincmd h`, `:wincmd j`, `:wincmd k`, `:wincmd l`: Moves to the left, bottom, top, and right window, respectively
- `gt`, `gT`: Moves to the next and previous tabs, respectively

We also used [vim-windowswap](https://github.com/wesQ3/vim-windowswap), a plugin that allows us to swap the content between two windows horizontally or vertically. We tested this plugin by typing the command `:WinSwap` followed by either `h` (for horizontal swap) or `v` (for vertical swap).

Finally, we saved the current session by using the command `:mksession`, which creates a Vim script file containing the entire session. To restore the session, we simply typed `vim -S` followed by the name of the file created by `:mksession`.

By employing these techniques and plugins, we can make navigating between multiple files in Vim much more efficient and productive. Keep practicing, and you will become a Vim master in no time!


[Next Chapter](09_Chapter09.md)