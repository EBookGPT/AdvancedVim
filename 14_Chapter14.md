# Chapter 14: Vim Buffers, Marks and Jumps

Welcome back to our journey through the world of Advanced Vim! In the last chapter, we explored the art of folding in Vim. However, in this chapter, we will be diving into the concepts of Buffers, Marks and Jumps - three fundamental elements in Vim to master the art of editing.

Joining us in this chapter is our special guest Steve Losh, a developer and Vim expert, who has provided valuable insights into using these features effectively to enhance and streamline your editing process.  

In this chapter, we will go through some of the essential keyboard shortcuts, commands and techniques to help you leverage the power of Vim's Buffers, Marks and Jumps. We will explore how to move quickly between different files, create new buffers and manage them efficiently, mark important locations in a file, and navigate through the code effectively using Jumps. 

By the end of this chapter, you will have gained a deep understanding of the capabilities of Buffers, Marks and Jumps, along with the skills to use them effectively in your workflow. You'll be able to take advantage of the immense power of Vim to navigate and edit complex codebases with ease, and save yourself a ton of time and effort in the process.

So let's dive in and explore the wonderful world of Buffers, Marks and Jumps in Vim!
# Chapter 14 Exercises: Vim Buffers, Marks and Jumps

Congratulations on making it to the exercises section for Chapter 14 on Vim Buffers, Marks and Jumps! In this section, you'll have the opportunity to test your knowledge and skills on the topics covered in the chapter.

We've designed these exercises to help you gain practical experience navigating and manipulating files using Vim's Buffers, Marks and Jumps - both the essential commands and the more advanced techniques covered in the chapter.

Each exercise has clear instructions, and where necessary, hints are provided to help you along your way. And don't forget to pay attention to our special guest, Steve Losh, who has imparted his unmatched wisdom on the topic.

So what are you waiting for? Jump right in, and start building your expertise in Vim's Buffers, Marks and Jumps!

1. Creating and Managing Buffers
- Start by creating a new buffer using the :new command.
- Switch between your existing buffers using the :ls command and the :b buffer_name command.
- Close a buffer using the :bd command.
- (Bonus) Use the :ball command to display all open buffers in separate windows.

2. Working with Marks
- Set a mark on an important line using the m command.
- Jump to a mark using the ' character.
- View all existing marks using the :marks command.
- (Bonus) Use the :delmarks command to delete all marks.

3. Navigating with Jumps
- Jump to the last edited position in a file using the <C-o> command.
- Jump forward to the next edit position using the <C-i> command.
- View a list of recent jumps using the :jumps command.
- (Bonus) Use the g; and g, commands to navigate through a jump list.

Remember to refer back to the chapter and the Vim documentation as needed to help you complete these exercises. Good luck and have fun!
One of the exercises in Chapter 14 requires us to switch between buffers in Vim. In order to accomplish this, we can use the `:ls` command to list all open buffers and their corresponding buffer numbers. 

Then, we can switch to a specific buffer by using the `:b` command followed by the buffer number. For example, to switch to buffer number 3, we would use the command `:b 3`.

Here's an example of how this might look in practice:

```
:ls
  1 %a   "file1.txt"       line 1
  2      "file2.txt"       line 1
  3      "file3.txt"       line 1
  4      "file4.txt"       line 1
  5      "file5.txt"       line 1
: b 3
```

In this example, we first use the `:ls` command to list all open buffers. We see that we currently have five buffers open, with buffer number 3 being the file "file3.txt".

Then, we use the `:b` command to switch to buffer number 3. Once we execute the `:b 3` command, Vim will switch to the buffer with the file "file3.txt" and display its contents on the screen.

Remember that Vim's buffer commands can be incredibly powerful when used correctly. With a little practice, you can use them to easily switch between files, manage multiple files at once, and streamline your editing workflow.


[Next Chapter](15_Chapter15.md)