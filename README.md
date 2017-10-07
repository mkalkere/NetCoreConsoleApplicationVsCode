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
dotnet new console -o "ConsoleApplication"
```
_1. _``dotnet new console``_ : scaffolds the console application template._ 

_2. _``-o "ConsoleApplication"``_ : inputs the folder in which to scaffold the files into._

![Image](https://drive.google.com/open?id=0BxD93dWLzjMSNzVVS2xRZTJlY3c)

Now you will have all the files created required for the Console Application.

####Step 2:
