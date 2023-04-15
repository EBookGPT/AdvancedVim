# Chapter 2: Vim Configuration, Settings and Options

Welcome to the second chapter of our Advanced Vim book! In this chapter, we'll be discussing one of the most important aspects of Vim: its configuration, settings, and options.

Vim is an incredibly customizable text editor, with countless configuration options that can be tweaked to fit your specific needs and workflow. Whether you're a seasoned Vim pro or a newbie just getting started with this powerful editor, mastering Vim's settings and options is key to unlocking its full potential.

In this chapter, we'll cover everything from basic settings like line numbers and syntax highlighting, to more advanced options like autocommands and custom keybindings. We'll explore the Vim configuration file and learn how to modify it to suit our needs. 

We'll also delve into some more esoteric settings, uncovering hidden gems that can make your Vim experience even smoother and more efficient. Did you know, for instance, that Vim has a built-in spell checker that can highlight typos as you type? Or that it can highlight visually-indented blocks of text with a single keystroke? 

Through a combination of explanation, examples, and exercises, this chapter will guide you through the vast landscape of Vim settings and options, giving you the tools you need to truly make Vim your own. So grab your configuration file, open up Vim, and let's get started!
# Chapter 2 Exercises: Vim Configuration, Settings and Options

Congratulations on making it to the exercises portion of this chapter! This is where you get to put your newfound knowledge of Vim's configuration, settings, and options into practice.

Below, we've provided a variety of exercises designed to challenge you and help you develop your Vim customization skills. Each exercise should be completed using only Vim commands and configuration modifications - no cheating with outside tools or plugins!

Remember, the key to mastering Vim's configuration is practice and experimentation. Don't be afraid to tinker with settings and options to see what works best for you.

Alright, let's dig in!

## Exercise 1: Basic Settings

For this exercise, we'll start with some simple settings modifications. 

1. Turn on line numbers for all files.
2. Change the background color of the editor to a light grey.
3. Turn off mouse input (no clicking allowed!).

## Exercise 2: Advanced Settings

Next, we'll move on to some more advanced settings tinkering. 

1. Add a custom autocommand that automatically saves the current file whenever you switch to another buffer.
2. Change the default colorscheme to something more colorful and eye-catching.
3. Modify the format of the statusline to include your current Git branch name.

## Exercise 3: Custom Keybindings

Lastly, let's work on some custom keybindings to speed up your workflow. 

1. Map the `leader` key to the spacebar.
2. Create a new keybinding that toggles syntax highlighting on and off.
3. Map the `Ctrl + S` shortcut to save the current file (even though you've already got autocommands set up!).

Good luck with these exercises! Happy tinkering.
Sure! Here's an explanation of the code used to resolve Exercise 2, Question 1: 

**Add a custom autocommand that automatically saves the current file whenever you switch to another buffer.**

An autocommand is a Vim command that automatically triggers when a certain event occurs. In this case, we want to set up an autocommand that saves the current file whenever we switch to a different buffer. 

Here's the code to accomplish this: 

```
autocmd BufLeave * silent! wall
```

Let's break this down line by line: 

- `autocmd` tells Vim that we want to create an autocommand. 
- `BufLeave` is the event that we want to trigger the command. This event occurs when we leave the current buffer and move to another one. 
- `*` is a wildcard that tells Vim to apply this command to all filetypes. 
- `silent!` suppresses any output that Vim would normally give us. We don't need to see any messages confirming that the file has been saved.
- `wall` is short for `w all`, which is the command to save all open buffers to disk. This is triggered when the `BufLeave` event occurs.

Overall, this autocommand ensures that any time we leave the buffer we were just editing, it will automatically save that file, without us having to manually issue a save command. It's a small but helpful modification that can save us lots of time and hassle down the line!

I hope that helps clarify the code used in this exercise. Let me know if you have any other questions!


[Next Chapter](03_Chapter03.md)