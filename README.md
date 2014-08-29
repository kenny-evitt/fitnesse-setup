# README

## Overview

*FitNesse setup* is a set of files for setting-up [FitNesse](http://www.fitnesse.org/) and [fitSharp](http://www.syterra.com/FitSharp.html) for a .NET project.

## Installing

1. Download or clone the repo.
2. Copy the *FitNesse* folder somewhere in your project's path; I like doing so right in the project's root folder. You'll need to use [Robocopy](http://technet.microsoft.com/en-us/library/cc733145.aspx) or something similar as Windows Explorer doesn't support paths as long as some of the FitNesse files. [The files with too-long paths are actually self-tests for FitNesse itself so it's not much of a loss if they're not copied.] Here's an example command that can be run from Command Prompt to copy the files using Robocopy:


    `robocopy C:\where-you-downloaded-or-cloned\FitNesse . /e`

<ol>
<li value="3">Copy the <em>fitSharp</em> folder to the 'referenced assemblies' path for your project.</li>
<li>Add references to the <em>fit.dll</em> and <em>fitSharp.dll</em> assemblies in the <em>fitSharp</em> folder to Visual Studio project in your solution that will contain your integration tests.
</ol>

## Running FitNesse

Run the batch file *\FitNesse\release_x\run-fitnesse.bat* to start the FitNesse server and open the 'front page' in your default browser.