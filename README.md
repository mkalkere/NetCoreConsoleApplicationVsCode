# How to create a Console application in .Net Core and Visual Studio Code(VSCode) 


If you are used to Visual Studio for creating new projects then you will sure be wondering on how to create a new project in VS Code as there is no file new.

If you had ever encountered the above thought the don't worry you are not alone :wink:.

## Let's briefly take a look at how to create one.

### We would require the following installed:             
1. [.Net Core](http://www.microsoft.com/net/download/core)
2. [VS Code](https://code.visualstudio.com/) 

Once installed we can check to make sure that .Net Core is installed and the path variable is set properly be exexuting the below command in the command prompt.

```
dotnet --version
```
You should be getting the version installed depending on which version you installed:
```
Output:

2.0.0
```

#### Since we have set up the necessary tools required let's begin with creating the console application.

Before we actually start with [scaffolding](http://www.dictionary.com/browse/scaffold) the console application template. Let's try to understand briefly the tool which helps in Scafolding, Debugging and Building the .Net Core Application - [.Net CLI](https://docs.microsoft.com/en-us/dotnet/core/tools/?tabs=netcore2x) Tool.

In simple terms it's a cross platform tool which aids in developing the .Net Applications and other high level tools.
#### Step 1:

Open a ``Command prompt`` or a ``Terminal in VS Code`` (by clicking _``Ctrl+` ``_ ) and enter the below command
```
c:\> dotnet new console -o "ConsoleApplication"
```
_1. _``dotnet new console``_ : scaffolds the console application template._ 

_2. _``-o "ConsoleApplication"``_ : inputs the folder in which to scaffold the files into._


Now you will have all the files created required for the Console Application.

#### Step 2:
Switch the path to the folder _``ConsoleApplication``_ using the below command. 
```
c:\> cd ConsoleApplication
```

#### Step 3:
Enter the below command to open the _ConsoleApplication_ project in _VS Code_
```
c:\ConsoleApplication> code .
```
This will open the _ConsoleApplication_ project in the _Visual Studio code_. VS Code will prompt you to install the C# extension rightly identifying the project type which you have opened.

Go ahead and install the [C#](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp) extension from Microsoft which provides the great development and productivity experiance like Syntax Highlighting, Intellisense, Debugging Support and many more.

#### Step 4:
Configure VS Code to build and debug the project.

we need to configure the VS code to tell it how to compile and debug the applications. For this it uses 2 files.

Usually VS Code will prompt you to add the missing assets for debug and build automatically when you open any project and if you have C# extension installed.

We will not be discussing on how to add the required files to build and debug the project here. you can find more details on this over [here](https://github.com/OmniSharp/omnisharp-vscode/blob/master/debugger.md).

* Task.json 
* Launch.json

Open launch.json file and find the section _``"name": ".NET Core Launch (console)"``_

Replace the belwo line:

_``"program": "${workspaceRoot}/bin/Debug/<insert-target-framework-here>/<insert-project-name-here>.dll",``_

With:

_``"program": "${workspaceRoot}/bin/Debug/netcoreapp2.0/ConsoleApplication.dll",``_

Now you are all set to debug your Console application in _Visual Studio Code_

#### Step 5:
* Place a break point in program.cs file either by clicking on the line of code where you want the debug to break and pressing F9 key or by clicking on the space to the left of the line number.

* Press F5 to begin debug yor code.
