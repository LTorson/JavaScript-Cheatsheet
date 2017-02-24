# JavaScript-Cheatsheet
JavaScript based Cheatsheet with sources from Treehouse

**Useful resources:** 
https://developer.mozilla.org/en-US/

---

####Placing Scipts

```Script tag = <script src="script.js"></script>```
placed either before the closing ```</head>``` or ```</body>``` tags; benefit of placing before the body tag is that it will let the browser load and display any HTML before running the JavaScript.

---

```Alert("Hello World");``` = Displays an alert window with a message inside the quotes for the user to then close via pressing "OK". 

---

```document.write("Hello World");``` = Writes out a message to the html on the page.

----

#### Web Browsers:
When the browser executes a line of programming code, a dialogue box appears on the screen. 

All browsers have JavaScript Console just like CSS has the Inspect tool. 

##### Chrome Console Keyboard Shortcuts
* Windows: ```Ctrl + Shift + J```
* Mac: ```Cmd + Option + J```

##### Firefox Console Keyboard Shortcuts
* Windows: ```Ctrl + Shift + K```
* Mac: ```Cmd + Option + K```

##### Internet Explorer Console Keyboard Shortcuts
* Windows & Mac: ```F12``` key

##### Safari Console Keyboard Shortcuts
*  ```Cmd + Option + C```

----

####Console.log

```Console.log("Hello World")```; = Let's you place in your JavaScript code to display a message in your console. This is good for Debugging code and checking if a piece of code if reaching that console.log();

----

**Syntax Error** = A grammicalerror located in your code that is stopping the code from executing correctly.

----

####Variables

**Variables || Var = Stored data**.  For example: ```var score = "0";```

data || content placed on the right of a variable, will be getting stored into the var on the left. 
```var message = 'Hello ';```

```var message = "Hello";```  // String based variable

**alert(message);**


```message = "Hello World";```  We don't need to put a var in front of this one as we only do that when we create the first initial variable with the same name. 

variables are interchangeable throughout your code. 

##### Use descriptive naming conventions: 

Bad Naming                    Good Naming
```var p = "Player";```             ```var PlayerScore = "PlayerOne";```

----

#### Two Common Value Types

**Numbers** = Used for making calculations, adding, subtracting - keeping track of scores and more. 

**Strings** = Used for words, sentences, and other text. For Example: ```alert("String inside quote marks");```
Strings are made up of text within quotation marks, either single or double quotes. 
**Escape Character || "\"** = placed before a single quot mark to treat it like a normal character with no special powers.
```message = 'She/'s a quot mark'';```

----

####Spacing

**Spacing** = When programming it's good to add space, however having too much or too little space can be a bad thing. For example: 

**Bad Spacing**: ```vardaysInWeek =7; || var     days     In     Week =      7;```
**Good Spacing**: ```var daysInWeek = 7;```  // as you can see, we only separate space when it's needed to divide different areas.

----

####Prompt();

```Prompt command || prompt("Please click Me");``` = Like the ```alert("Hello World");``` command, this will be a popup box however the prompt will ask the user to interactive without via either filing out an input field or simply clicking a button in order to carry on. 

**Prompt** captures the users response and stores the value. We can then use this stored information and use it somewhere else. In programming speak, this is referred to as a **Returned Value**. 

```var visitorName = prompt("What is you name");```   


alert(**visitorName**);

The prompt command will in the end return a string. 

----

####Combining strings

**Combining strings** = in order to place multiple string values inside quotation marks, you simple divide them with a + symbol.
For example:
* ```var visitor = prompt('what is you name?');```
* ```var message = 'Hello ' + visitor + '.' + 'welcome';```
* ```document.write(message);```

code can also be more easier to read when you use smaller statements rather than one long statement. 
For Example: 
* ```var visitor = prompt('what is you name?');```
* ```var message = 'Hello ' + visitor + '.' + 'welcome';```
* ```message = message + "This is added onto the end";```
* ```document.write(message);```

we are basically accessing the stuff in the first variables and then adding onto it once we've hit the second request indicating changes to the message variable before then writing out on the page. 

This method is also called **Concatenation** - The combining of strings. 

---

####.length();

**Length phrase || .length** = Finding out how many characters are made up from the data you passed into it. 
For Example:
* ```var lengthExample = 'Welcome';```
* ```console.log(lengthExample.length);```

separating and understanding a call.
**message.length ===   Object | Accessing a property | Property**

A property is kinda like a variable, it holds information. A string's length property contains a number, you can use the length property on any string, even a literal collection of charters inside a quote. Removing one character will change the length value. 
Just like a variable, properties are dynamic and can change. 

---

####Methods

**Methods || .example();** = The parentheses at the end of a property indicate that it's also a method.  A command you can perform on a string. 

For Example: 
* ```console.log( "TEST".toLowerCase() );``` // "test"
* ```document.write();```

---

####Basic application to merge two prompt inputs together to give you a subTotal.
 
```var jobOne = Number(prompt("How many hours have you worked on job 1?"));```
```var jobTwo = Number(prompt("How many hours have you worked on job 2?"));```

```var total = jobOne + jobTwo;```


```document.write("You've worked" + " " + total + " " + "Hours");```

---

####Working with Numbers

Numbers can be **whole numbers**, referred to as integers, like 5, 0, -100, 9999. OR even using **decimal points** or **scientific notation**. 

Numbers can be placed in variables as well as stings.
For example. 
```var pi = 3.141592653589793;```

Unlike strings however, you don't put quote marks around a number declared inside a variable object. If you do, you have string and not a number. 

**Operators:**
* Adding two numbers together, you'd use the **+** symbol. || 4 + 3; \\ **Plus**
* Subtracting two numbers together, you'd use the **-** symbol. || 4 - 3;  \\ **Minus**
* Multiplying two numbers together, you'd use the * symbol. || 4 * 3; \\ **Asterix**
* Dividing two numbers together, you'd use the **/** symbol. || 4 / 3; \\ **Divider**

**Shorthand Versions**
* ```score = score + 10; || score += 10;```
* ```score = score - 20; || score -+ 20;```
* ```score = score * 5; || score *= 5;```
* ```score = score / 2; || score /= 2;```

---

**Object Notation**

Creating Sub Methods within a function so you can better control and run your functions with as many sub methods as you want.

```var $navigationList = $('.navigation__list');```
```var navHeight = { ```
   ``` init: function() { ```
       ``` $navigationList.css({ ```
           ``` 'min-height': $navigationList.height(), ```
           ``` 'max-height': $navigationList.height() ```
       ``` }); ```
   ``` }, ```
   ``` reset: function(){ ```
       ``` $navigationList.css({ ```
           ``` 'min-height': '0', ```
          ```  'max-height': 'none' ```
      ```  }); ```
   ``` } ```
``` }; ```
