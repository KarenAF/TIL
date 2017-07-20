To run a C# file from the Terminal, youll need to have Mono downloaded. http://www.mono-project.com/ To check if it's downloaded, type 'mono' and youll see a list of Monno command options. You may need to download an older version, if this doesn't work. (Try version 4.3.2 from  https://download.mono-project.com/archive/) 

Quit your terminal and re-open.

To run a C# file, cd into the folder that the C# file is in. Type mcs filename.cs and press enter. Nothing will happen yet. Then type mono filename.exe. Then your program will run. Replace filename with whatever your file is called. So if your file is called Palindrome.cs, youll type: 
```mcs Palindrome.cs
mono Palindrome.exe```
