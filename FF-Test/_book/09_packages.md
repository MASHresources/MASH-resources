# Packages

## Introduction 

This document is part of our "First Steps in ***R***" resources. It is assumed that the reader has installed ***R*** and ***RStudio*** and understands how to type commands in the console. If you would like to recap these topics, the documents and videos are on the MASH website.

## What is a Package?

***R*** is a collaborative language, a little like Wikipedia. Anyone can write new functions or create new objects and make them available for other ***R*** users in a package. You can think of a package like an app for a smartphone. Which packages you download will depend on what you want to do in ***R***. There are two ways of installing packages, either using menus or in the console window using ***R*** commands.

## Installing Packages from Menus

In the bottom right window of ***RStudio***, click on the "**Packages**" tab. In this tab you can see a list of all the packages which are already installed.

<figure>
    <center>
        <img src="media/09_media/media/09_media/H_Installing_Packages_in_R_fig1.png" width="900" title="Figure 1"
             alt="An image showing the bottom right window in RStudio, with the 'Packages' tab selected. Under 'User Library', there is a list of four packages: 'askpass', 'assertthat', 'backports' and 'BH'. 'Packages' is cricled.">
        <figcaption style="text-align:center">
            Figure 1: The "Packages" tab in the bottom right window in <b><em>RStudio</b></em>.
        </figcaption>
    </center>
</figure>

To install a new package that is not in the list, click "Install", which opens up the "Install Packages" dialogue box and allows you to download packages from the CRAN repository. CRAN stands for "Comprehensive R Archive Network." This is a website which stores ***R*** packages for ***R*** users to download. You can think of it as the ***R*** version of the App store on a smartphone.

<figure>
    <center>
        <img src="media/09_media/media/09_media/H_Installing_Packages_in_R_fig2.png" width="800" title="Figure 2"
             alt="An image showing the bottom right window in RStudio, with the 'Packages' tab selected. Under 'User Library', there is a list of six packages: 'abind', 'askpass', 'assertthat', 'backports', 'base64enc' and 'BH'. 'Install' in the top ribbon of the window is cricled.">
        <figcaption style="text-align:center">
            Figure 2: The "Install" button in the "Packages" tab in the bottom right window in <b><em>RStudio</b></em>.
        </figcaption>
    </center>
</figure>

Type the name of the package you want to install. In this case we will install the package <code style="color: blue;">ggplot2</code>. This is an often-recommended package which contains functions for making elegant graphs and charts.

<figure>
    <center>
        <img src="media/09_media/media/09_media/H_Installing_Packages_in_R_fig3.png" width="400" title="Figure 3"
             alt="An image showing the 'Install Packages' dialogue box in RStudio. In the box under 'Packages (separate multiple with space or comma):', 'ggplot2' is typed in.">
        <figcaption style="text-align:center">
            Figure 3: The "Install Packages" dialogue box in <b><em>RStudio</b></em>.
        </figcaption>
    </center>
</figure>

When we click "**Install**" we will see the progress of the installation in the console. Depending on the package, the installation can take a few minutes. When the installation is finished we will receive a confirmation message in the console.

Our new package should now appear in the list of packages in the "Packages" tab.

<figure>
    <center>
        <img src="media/09_media/media/09_media/H_Installing_Packages_in_R_fig4.png" width="900" title="Figure 4"
             alt="An image showing the list of packages in the 'Packages' tab in RStudio. There are five packages listed: 'fansi', 'farver', 'ggplot2', 'glue' and 'gtable'.">
        <figcaption style="text-align:center">
            Figure 4: The list of packages, with <code style="color: blue;">ggplot2</code> added, in the "Packages" tab in <b><em>RStudio</b></em>.
        </figcaption>
    </center>
</figure>

## Installing Packages Using the Console

The command <code style="color: blue;">install.packages()</code> can be used to perform the same operation as described above. The name of the package to install should be in inverted commas like so:

<center>
    <code style="color: blue;">install.packages("ggplot2")</code>
</center>

## Using Your New Package

Once a package has been installed in ***R***, you will then need to tell ***R*** that you want to use it. In the list of packages you will notice that some packages have a tick while most do not. The package we have just installed, <code style="color: blue;">ggplot2</code>, does not have a tick. This means that the package has been downloaded (installed) but ***RStudio*** is not interacting with it.

<figure>
    <center>
        <img src="media/09_media/media/09_media/H_Installing_Packages_in_R_fig5.png" width="900" title="Figure 5"
             alt="An image showing the list of packages in the 'Packages' tab in RStudio. There are five packages listed: 'forcats', 'foreign', 'ggplot2', 'glue' and 'gtable'. The empty box next to 'ggplot2' is circled.">
        <figcaption style="text-align:center">
            Figure 5: The empty box next to <code style="color: blue;">ggplot2</code> in the "Packages" tab in <b><em>RStudio</b></em>.
        </figcaption>
    </center>
</figure>

If we want to use the functions or objects from the new package we need to tell ***R*** to access it using the <code style="color: blue;">library</code> command like so:

<center>
    <code style="color: blue;">library(ggplot2)</code>
</center>

The functions and objects in the new package are now available to use and a tick has appeared in the list of packages.

Alternatively, we can find the package in the list of packages and tick the box using the mouse. You will notice that the <code style="color: blue;">library()</code> command appears in the console window.
