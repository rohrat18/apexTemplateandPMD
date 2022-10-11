                             **CLASS TEMPLATE AND APEX PMD**

The extension provides the basic class and test class template. Apart from these templates there are few manual steps to be done in order to run Apex PMD containing our own customizable rulesets.

# Features
1. It provides template of the classes that should be followed while creating a new class or test class.
2. It gives you the overview of the errors where we have done mistake and it will not allow us to deploy to org unless we correct them.
# How to use
1. Inorder to use the class template type **"!apextemplate"** and for test class type **"!testtemplate"** you will get the code then continue coding.
2. Create a folder like "rulesets\apex\apex-ruleset.xml" in the workspace you are currently working and then type **"apexruleset"**.
3. Press _"Ctrl+Shft+P"_ and then start typing Task... you will get a list of task functions select "Task: Configure Default Build task" and once you select that will get a window opened up there type **"task"**. This step of configuring default build task is onle first time, later whenever you want to run this default build task just press _"Ctrl+B"_.
![Screenshot](https://github.com/rohrat18/apexTemplateandPMD/blob/master/images/task%20configure.jpg)

4. The error after running Apex PMD can be seen in the form of *.html*,* .txt* or *.xlsx*. We can change the format of our report file how we want to see those errors for easy purpose with detailed information. For example in the task template we can see that there is **Output.html** above that there is a format "-f", here we can specify what format we need for our report file.
`"-f",
"html",
"-R",
"rulesets\\apex\\ruleset.xml",
"--report-file",
"Output.html"`

5. For more information refer this link https://github.com/rohrat18/apexTemplateandPMD



                