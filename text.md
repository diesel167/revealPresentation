What is Typescript? It is an open-source programming language developed and maintained by Microsoft. It is a strict syntactical superset of JavaScript, and adds optional static typing to the language.
Since Typescript is just a language extension, browsers can't interpret it. 

The Compiler (or more exact Transpiler) transpiles the typescript code to Javascript-Code that the browser can easy  interpret. Converting from TypeScript to JavaScript is called compiling here. TypeScript compiles to clean, simple JavaScript code which runs on any browser, in Node.js, or in any JavaScript engine. TypeScript is a syntactic sugar for JavaScript. Every JavaScript program is also a TypeScript program.
TS is a strict, static, explicit or implicit typing language. What is mean?

Strict typing is case when we couldn’t
to add, subtract, multiply different types of data (for example string and number) while JS independently will transform data to one type automatically.

Static typing means that types are assigned to data at compile time instead of running time in JS which calls dynamic typing.

Explicit or implicit typing means that we may assign types to variables when we write code or may not assign and the types will be assigned automatically like in JS.

BENEFITS

What are benefints?
The ability to strict describe each element of the application - this excludes the possibility of incorrect implementation or incorrect calling of methods.
Makes developers think about  logic (for example, in methods) before implementation.

It does not give the opportunity to change one piece of the application, breaking the other
The ability to describe the scope of class properties. That is clear.

Because of strict syntax it may be necessary to write fewer tests.

You can configure the project in such way that any non-compiled code (in fact, a code with a syntax error) cannot be committed.

LIMITATIONS

To use some external tool (like “library” or “framework”), then the signature of each of the methods of each module of this tool must be described to the compiler does not throw errors (because it will not know about your tool). It makes the development process longer and make developers to pay more attention.

Probably the biggest minus (possibly temporary) is little number of specialists on the market. Now there are almost  no specialists who know this language. This is bad, because any solid project moves to the support stage, and in the case of the loss of specialists, it will be more difficult to find a replacement for them. It is more difficult to learn this language and to solve unique problems. This conclusion based on Github statistics - only ~ 6k repositories were created with TypeScript code against ~ 1.4kk in JavaScript.


More time is spent on development, compared to JavaScript. This is because in addition to the class implementation, it is necessary to describe all the interfaces involved it is needed from developers more accuracy for it.

Lets start.
That is the code which is used for installing TS to your project. First line is well known to us. The second line is the command to compile sourse.ts file. If there are any mistakes you will see them.

Let's see how it looks

At this slide we can see all variables types . Everything is clear with names.  Note at tha appearance of multitype declaration. Two types of variable can be assigned to ‘multitypeVar’.

You also can create your own types throw ‘type’ keyword.

Now you can see how to create objects in TS. It is very similar to javascript but now we write the variables types
Let’s see the difference on another example. There is the same function but at the top of slide it is on js and at the bottom it is on ts. See? We don’t need to write tests for incorrect var types now because ts will check it itself.
Now speak about classes
Let’s create new class Mamal. Don’t forget to specify types for variable because if we wouldn’t do that typescript will be useless.
Create another class Cat which extends Mamal. We also have to specify method type it will be the type of return data.
Some template for our case when transform ts to js.
And finally, let's see what the previously written code looks like in native Js. No types as you can see but typescript doesn’t sleep, it check the types.
What is interface? It is type-description of our object’s template for object creating in future. If we create object we could to set it type to some interface. Let’s look for examples.
Note that if we want some filed not to be required we should specify it with question-symbol.

Also pay attention on readonly keyword. It is mean that you can change variable only one initial time. Every next time the variable will be only for reading.
Create interface IUser. And after create the object employee with type of IUser. See? Now type of employee id = number as we have written earlier in the IUser.
If the field of object won’t return any value we set the type to void;

Great. Continue

At the final I want to note TSlint that is the brother of our well known ESlint. Write the code on the slide to install and init TSlinter. tslins.json will be created which would contain all rules for tslint.

