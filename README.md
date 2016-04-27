# JavaScript-Cheatsheet
JavaScript based Cheatsheet with sources from Treehouse

---

```Script tag = <script src="script.js"></script>```
placed either before the closing **</head>** or **</body>** tags; benefit of placing before the body tag is that it will let the browser load and display any HTML before running the JavaScript.

---

```Alert("Hello World");``` = Displays an alert window with a message inside the quotes for the user to then close via pressing "OK". 

---

```document.write("Hello World");``` = Writes out a message to the html on the page.

----

##### Web Browsers:
When the browser executes a line of programming code, a dialogue box appears on the screen. 

All browsers have JavaScript Console just like CSS has the Inspect tool. 

##### Chrome Console Keyboard Shortcuts
* Windows: Ctrl + Shift + J
* Mac: Cmd + Option + J

##### Firefox Console Keyboard Shortcuts
* Windows: Ctrl + Shift + K
* Mac: Cmd + Option + K

##### Internet Explorer Console Keyboard Shortcuts
* Windows & Mac: F12 key
* Safari Console Keyboard Shortcuts
* Cmd + Option + C

----

````Console.log("Hello World")````; = Let's you place in your JavaScript code to display a message in your console. This is good for Debugging code and checking if a piece of code if reaching that console.log();

----

**Syntax Error** = A grammicalerror located in your code that is stopping the code from executing correctly.

----

**Variables || Var = Stored data**.  For example: ````var score = "0";````

````var message = "Hello";````  // String based variable

**alert(message);**


````message = "Hello World";````  We don't need to put a var in front of this one as we only do that when we create the first initial variable with the same name. 

variables are interchangeable throughout your code. 

##### Use descriptive naming conventions: 

Bad Naming                    Good Naming
````var p = "Player";````             ````var PlayerScore = "PlayerOne";````

----

#### Two Common Value Types

**Numbers** = Used for making calculations, adding, subtracting - keeping track of scores and more. 

**Strings** = Used for words, sentences, and other text. For Example: ````alert("String inside quote marks");````
Strings are made up of text within quotation marks, either single or double quotes. 
**Escape Character || "\"** = placed before a single quot mark to treat it like a normal character with no special powers.
````message = 'She/'s a quot mark'';````

----

**Spacing** = When programming it's good to add space, however having too much or too little space can be a bad thing. For example: 

**Bad Spacing**: ````vardaysInWeek =7; || var     days     In     Week =      7;````
**Good Spacing**: ````var daysInWeek = 7;````  // as you can see, we only separate space when it's needed to divide different areas.

----

````Prompt command || prompt("Please click Me");```` = Like the ````alert("Hello World");```` command, this will be a popup box however the prompt will ask the user to interactive without via either filing out an input field or simply clicking a button in order to carry on. 

**Prompt** captures the users response and stores the value. We can then use this stored information and use it somewhere else. In programming speak, this is referred to as a **Returned Value**. 

````var visitorName = prompt("What is you name");````       

**alert(visitorName);**

----

