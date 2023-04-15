# Chapter 4: Advanced Editing Commands and Tools

Welcome back Vim enthusiasts! In the previous chapter, we explored some advanced cursor movement techniques that can help you navigate through large and complex files like a pro. In this chapter, we will delve into the realm of Advanced Editing Commands and Tools. Here, we'll learn some powerful techniques to manipulate text and code snippets more efficiently.

We also have a special guest for this chapter- the legendary Vim Plugin author, Tim Pope. He has contributed to numerous open source Vim plugins, including Vdebug, Fugitive, and Tim Pope Text Object. Tim will share invaluable insights into his development experiences and how Vim became the go-to editor for many programming languages.

We all find ourselves writing code that needs more than just basic editing. We need to refactor, re-structure, and re-organize our codebase. Using Vim's advanced editing commands, we can significantly improve the overall development workflow. Without further ado, let's dive in and explore some exciting advanced editing techniques.

Are you ready to enhance your productivity? Let’s get started!
# Chapter 4: Advanced Editing Commands and Tools - Exercises

Congratulations on reaching the end of the Advanced Editing Commands and Tools chapter. It’s time to test your knowledge and cement your learning by completing the following exercises. We’ve included examples and code snippets to help you work through the exercises efficiently.

## Exercise 1: Tim Pope Text Objects

In this exercise, you will utilize a plugin written by Tim Pope, the creator of popular Vim plugins Vdebug and Fugitive. The plugin is known as Tim Pope Text Objects, which provides additional text objects above and beyond Vim's built-in text objects.

1. Install Tim Pope Text Objects using your preferred plugin manager. To use *Vundle*, add `Plugin 'tpope/vim-textobj-user'` to your `.vimrc` file and then run `:PluginInstall` in Vim.

2. Navigate to a file containing some code you want to refactor.

3. Use the `ci` command with the `ip` text object to replace the inner paragraph of text. For example, running `cip` while the cursor is on a paragraph of text will delete the current paragraph and place you in insert mode. 

   ```vim
   " Old code
   def some_function():
       print("Hello World!")
       print("Goodbye World!")
       print("Thanks for stopping by!")

   # To refactor, place the cursor anywhere within the paragraph you want to change, then press cip
   def some_function():
       print("Hello Universe!")
   ```
4. Use the `vis` text object to manipulate text spanning across multiple lines. This is more tolerant than Vim's built-in `vip`. Place your cursor inside any paragraph of text and hit `vis`.

   ```vim 
   # Original text
   def some_function():
       x = 3
       y = 4

   # Delete the two lines in-between, place the cursor on any word and type `visd`
   def some_function():
       # two blank lines
   ```

## Exercise 2: Tabular plugin

In this exercise, you will learn how to use the Tabular plugin to make your code look more professional and well-organized.

1. Install the Tabular plugin using your preferred plugin manager. To use *Vundle*, add `Plugin 'godlygeek/tabular'` to your `.vimrc` file and then run `:PluginInstall` in Vim.

2. Navigate to a file containing code with poorly-aligned text that could be reformatted.

   ```vim
   # Before refactoring
   def function(x,y,z):
       result = x+ y - 2*z
   return result
   ```

3. Align all the `=` signs in the code by typing `:Tab /=` in normal mode.

   ```vim
   # After refactoring
   def function(x,y,z):
       result = x + y - 2 * z
       return result
   ```

Congratulations! You have completed the advanced editing commands and tools exercises.

We hope you found these exercises informative and challenging. Don't forget to take a break and stretch your fingers before your next Vim editing session.
Sure, let me help you understand the code used in the exercises!

#### code for Exercise 1:

`ci` stands for "change inside" and is followed by a text object. In our case, `ip` stands for "inner paragraph". So, `cip` changes the text from inside the current paragraph, which could come in handy when refactoring text.

`vis` text object highlights the text in a more smarter way than Vim’s default text object `vip`. It selects the visual block mode within the text, ignoring extra white spaces and indentation issues. Using `vis`, you can easily manipulate text spanning across multiple lines.

#### code for Exercise 2:

Tabular plugin helps to align text in specific patterns or tabs. The command `:Tab /=` will align all equal signs in the selected text. By separating the function parameter with spaces and aligning the equal signs (this is one way, but there are many ways), we can increase our code's readability and overall aesthetic. 

I hope this explanation clears up any questions you had. Keep practicing and have fun with Vim!


[Next Chapter](05_Chapter05.md)