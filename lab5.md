# Lab Report 5 - Putting it All Together (Week 9)
## Part 1 – Debugging Scenario

**Original Post from Student:**

Title: Weird Compilation Status Check

Category: Skill Demonstrations 

Description:
Hi, I'm practicing for skill demo 3 and I had a question about exit codes. I have a simple program that checks the compilation status of the main function, but the value is always 0 even when there are compilation errors. 

Here's the program with the error: 

![image](Error.png)

This was the ouput: 

![image](OutputError.png)

And here's the same code with no errors:

![image](NoError.png)

With the following output: 

![image](OutputNoError.png)

This was my code structure by the way: 

![image](Structrue.png)

**Response from TA:**

Hey there! It looks like you're trying to check the compilation status using echo <code>$?</code>. However, you should keep in mind that using echo `<code>$?</code>` after compiling it, will default the value back to 0 automatically. Instead, you should check the value of `<code>$?</code>` without echoing it.

Try this:

![image](TAFix.png)

Let me know if this resolves the issue and gives you the correct compilation status!

## Part 2 – Reflection
