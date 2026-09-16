# First interactions with R and RStudio

## Introduction 

This document is part of our "First Steps in ***R***" resources. It is assumed that the reader has downloaded ***R*** and ***RStudio***. No other pre-knowledge is required.

Most of the time we are used to interacting with a computer through a Graphical User Interface (GUI) (i.e. with folders, files, windows etc). In ***R*** and ***RStudio***, we type instructions (code) instead. The window the instructions are typed into is called the console. Of course, we must type our instructions in a way the computer will understand - this is why it's called a programming *language*. This is the way computers were operated before the development of GUIs. ***R*** is a programming language which has been developed specifically for doing statistics. ***R*** and ***RStudio*** are pieces of software which allow the computer to read the code we type and execute it (i.e. follow the instructions).

## Opening ***R***

If you open the ***R*** software you will get a window in which you can type code. This is the console. It is possible to use the ***R*** package to do statistics with ***R*** but ***RStudio*** is much more friendly to use. ***RStudio*** is called an Integrated Development Environment (IDE) for ***R***. Note that for ***RStudio*** to work, it requires that ***R*** is also installed. Because of its ease of use, once you've used ***RStudio***, you will probably find you never open ***R*** again! All of the materials in this series use ***RStudio*** for this reason.

## First Opening ***RStudio***

When you open ***RStudio*** for the first time there will be three windows. The one on the left is the console. You can type code directly in here and ***RStudio*** will follow your instructions as soon as you press return. One thing ***R*** can do is simple calculations like a calculator. You can experiment by typing calculations in the console. If you type <code style="color:blue;">4+6</code> and press return, ***R*** will give you the answer $10$.

<figure>
    <center>
        <img src="media/03_media/B_First_Time_Opening_R_and_RStudio_fig1.png" width="900" title="Figure 1"
             alt="An image showing RStudio when it is opened for the first time. There are three windows: the one on the left is the console, the one on the top right shows the 'Environment' and the one on the bottom right shows files that can be selected. In the console, '4+6' is typed in and '10' is outputted.">
        <figcaption style="text-align:center">
            Figure 1: <b><em>RStudio</b></em> when it is opened for the first time.
        </figcaption>
    </center>
</figure>

If you'd like to carry out other calculations, here are the ways you must enter them into ***RStudio*** for some simple operations.

| Arithmetic Operation | R Code |
| :---: | :---: |
| $4+6$ | <code style="color:blue;">4+6</code> |
| $6-4$ | <code style="color:blue;">6-4</code> |
| $4 \times 6$ | <code style="color:blue;">4*6</code> |
| $4 \div 6$ | <code style="color:blue;">4/6</code> |
| $4^{6}$ | <code style="color:blue;">4^6</code> |
| $\mathrm{e}^{4}$ | <code style="color:blue;">exp(4)</code> |
| $\log_{10} (4)$ | <code style="color:blue;">log10(4)</code> |
| $\ln(4)$ | <code style="color:blue;">log(4)</code> |

Note that you cannot go back and delete text you have put in the console. If you've never done any coding at first this may seem strange but you'll get used to it quickly.

## Inputting Code Using a Script

A Script is the name for some code that has been written and which we want ***R*** to execute for us. You can write a script, edit it, save it then open it in ***RStudio*** and run it whenever you like. ***RStudio*** will let you let you edit your script until you're happy with it and then run all or just some of it by highlighting and clicking run. If you choose "**Save As**..." in the file menu (as you would when saving, say, a ***Word*** document) the script is what gets saved. To create a **Script file** for the first time, in ***RStudio***, click "**File**" then select "**New File**" and "**R Script**."

<figure>
    <center>
        <img src="media/03_media/B_First_Time_Opening_R_and_RStudio_fig2.png" width="800" title="Figure 2"
             alt="An image showing how to create a Script file in RStudio for the first time. In the top left corner, the 'File' tab is selected, then 'New File' is selected from the drop-down menu and 'R Script' is circled at the top of the next drop-down menu.">
        <figcaption style="text-align:center">
            Figure 2: How to create a Script file in <b><em>RStudio</b></em> for the first time.
        </figcaption>
    </center>
</figure>

A fourth window opens up on the top left in ***RStudio***. Try typing a few calculations in here. You will see that ***RStudio*** will let you type without carrying out any of the calculations. See what happens if you highlight the text and click "**Run**."

<figure>
    <center>
        <img src="media/03_media/B_First_Time_Opening_R_and_RStudio_fig3.png" width="900" title="Figure 3"
             alt="An image showing the fourth window, for scripts, in RStudio. The calculations '4+6', '7*5' and 'log10(100)' are typed into the window and are all highlighted. In the top right corner, the 'Run' button is circled.">
        <figcaption style="text-align:center">
            Figure 3: The fourth window, for scripts, in <b><em>RStudio</b></em>.
        </figcaption>
    </center>
</figure>

You should find that all the calculations are carried out at once in the console like so:

<figure>
    <center>
        <img src="media/03_media/B_First_Time_Opening_R_and_RStudio_fig4.png" width="500" title="Figure 4"
             alt="An image showing the console in RStudio, where there is the calculation '4+6', which outputs '10', the calculation '7*5', which outputs '35', and 'log10(100)', which outputs '2'.">
        <figcaption style="text-align:center">
            Figure 4: The calculations are carried out in the console in <b><em>RStudio</b></em> all at once when the script is run.
        </figcaption>
    </center>
</figure>

## The Environment

As we write code, we will create "***objects***". The word has a technical use in ***R*** programming which we will deal with in future worksheets. For now we will think of an object as being similar to a variable in algebra - i.e. a letter to which we can assign a value.

We can tell ***R*** that we are creating a new object using the "***assignment operator***":

<center>
    <code style="color: blue;">&lt;-</code>
</center>

You can think of this as an arrow. The name of the new object should go on the left and the definition goes on the right. So the code

<center>
    <code style="color: blue;">x &lt;- 3</code>
</center>

would create a new object called <code style="color: blue;">x</code> which is defined to have the value $3$. If we then type
    
<center>
    <code style="color: blue;">x+4</code>
</center>

We should find that ***R*** calculates $3+4$ and returns the answer $7$.

Type

<center>
    <code style="color: blue;">x &lt;- 3</code>
</center>

in the console then look in the top right window. You should find that it looks like this.

<figure>
    <center>
        <img src="media/03_media/B_First_Time_Opening_R_and_RStudio_fig5.png" width="900" title="Figure 5"
             alt="An image showing the top right window (the 'Environment') in RStudio. Under 'Values', 'x' and '3' are displayed inline.">
        <figcaption style="text-align:center">
            Figure 5: The top right window (the "Environment") in <b><em>RStudio</b></em>, where <code style="color: blue;">x</code> is defined to have the value $3$.
        </figcaption>
    </center>
</figure>

(Note: You can use <code style="color: blue;">=</code> as an assignment operator as well as <code style="color: blue;">&lt;-</code>. However, there is a technical difference in the way ***R*** reads <code style="color: blue;">=</code>. In most situations, either <code style="color: blue;">=</code> or <code style="color: blue;">&lt;-</code> can be used interchangeably but it is a good practice to stick to <code style="color: blue;">&lt;-</code> when defining a new object.)

When we are writing code we may want to define many new objects. These objects then exist in the ***R*** "Environment". As we create new objects, the top right window keeps a record of them for us. This helps us keep track and can help us ensure that we do not create two objects with the same name.

We can ask ***R*** to give us the same information by typing <code style="color: blue;">ls()</code> in the console. "ls" is short for list - we are asking ***R*** to list all the objects in the environment.

You can remove an object from the environment by typing

<center>
    <code style="color: blue;">rm()</code>
</center>

with the name of the object in the brackets.

For example,

<center>
    <code style="color: blue;">rm(x)</code>
</center>

would remove our variable <code style="color: blue;">x</code> from the environment.

You can delete all objects from the environment by clicking the broom icon in the top ribbon of the "Environment" window:
    
<figure>
    <center>
        <img src="media/03_media/B_First_Time_Opening_R_and_RStudio_fig6.png" width="900" title="Figure 6"
             alt="An image showing how to delete all objects from the environment in RStudio. The 'Environment' window is displayed and the broom icon in the top ribbon of the window is circled.">
        <figcaption style="text-align:center">
            Figure 6: How to delete all objects from the environment in <b><em>RStudio</b></em>.
        </figcaption>
    </center>
</figure>

Alternatively, you can type the following command in the console:

<center>
    <code style="color: blue;">rm(list=ls())</code>
</center>

(Note: we don't need to worry about the details of this command at the moment but in case you're interested: "rm" tells ***R*** to remove the thing in the brackets. The rest of the code tells ***R*** that it is going to remove an object which is a "list" and that list is called <code style="color: blue;">ls()</code>. A "list" is a category of object in ***R***. <code style="color: blue;">ls()</code> is specifically the list of everything in the environment.)

## The Bottom Right Window

There are several tabs in the window in the bottom right. For the moment we will only worry about two of them: "Plots" and "Help". If we ask ***RStudio*** to draw a graph or chart, it will appear in this window under this tab. If we ask ***RStudio*** for help - which we will often do when learning how to use a new piece of code - the answer will appear under the "Help" tab.

## Exercise

1. In the console, create an object called <code style="color: blue;">y</code> and give it the value $15$.  
2. Create another object called <code style="color: blue;">z</code> and give it the value $5$.  
3. Calculate <code style="color: blue;">y</code> divided by <code style="color: blue;">z</code>.  
4. Clear the environment and repeat the above by writing a script to do all three stages and running it.
5. Change the value of <code style="color: blue;">y</code> in your script to $20$ and run it again.

### Solutions
<details>
<summary>Solutions</summary>
    
1. <code style="color: blue;">&gt; y &lt;- 15</code>    

2. <code style="color: blue;">&gt; z &lt;- 5</code>  
<code style="color: blue;">&gt; y</code>   
<code>[1] 15</code>    
<code style="color: blue;">&gt; z</code>   
<code>[1] 5</code> 

3. <code style="color: blue;">&gt; y/z</code>    
<code>[1] 3</code>

4. Script:  
<code>y &lt;- 20</code>  
<code>z &lt;- 5</code>  
<code>y</code>  
<code>z</code>  
<code>y/z</code>  
And here it is run:  
<code style="color: blue;">&gt; y &lt;- 20</code>   
<code style="color: blue;">&gt; z &lt;- 5</code>  
<code style="color: blue;">&gt; y</code>   
<code>[1] 20</code>    
<code style="color: blue;">&gt; z</code>   
<code>[1] 5</code>    
<code style="color: blue;">&gt; y/z</code>    
<code>[1] 4</code>
</details>
