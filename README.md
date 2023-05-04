Download Link: https://assignmentchef.com/product/solved-csc33200-assignment-1-a-system-with-one-parent-process-and-two-child-processes
<br>
Assignment 1One of the philosophies behind Unix is the motto do one thing and do it well. In this spirit, each shell command usually has a very specific purpose. More complicated commands can be constructed by combining simpler commands in a pipeline such that the output of one command becomes the input to another command. The standard shell syntax for pipelines is to list multiple commands, separated by vertical bars (the pipe character).

Your task is to create a system with one parent process and two child processes where the children communicate using a pipe.

In the below example the output from the ls -F command is piped to input ofthe command.nl

Use fork(), one form of exec() functions, so that the first child will perform ls -F andpass the output to the second child using one direction pipe, so the second one canperform nl on the list of current directory contents. Later the second child process willprint to the screen the result (see example below). The parent process must wait for itsboth children.1 file1*2 file2*3 dir1/4 dir2/