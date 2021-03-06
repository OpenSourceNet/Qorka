Qorka
=======

![alt tag](http://3.bp.blogspot.com/-Jq-LXLknT-o/VZu1kXSJS3I/AAAAAAAAB7o/kd-Qy4_eKeA/s1600/mac-book-air-2%2Bcopy.png)

Ever wondered how awesome it would be if you could quickly assemble your own programming language (code interpreter) in minutes? or a program that allows you to code in Hindi, Spanish, French or any other language you ever wanted?

Qorka is an interpreter development platform from SourceNet which allows you to creatively put together your own programming interpreter with ease. This means that I can create my own programming syntax, by defining each function on the Qorka platform. And everytime I write a program with my own programming syntax (programming language) in a text editor and run it on Qorka, it will execute the file code according to the functions defined by you.

Qorka : Environment
=======

![alt tag](http://2.bp.blogspot.com/-rCPA4VoA3Oc/VZu7e23nhUI/AAAAAAAAB8o/u3t4LKZUtC8/s1600/summer%2Bjam%2Bseries.jpg)

Qorka is completely written in Python and requires knowledge in Python programming to operate. To get started, first open the Qorka code file, "qorka_mac.py" for Mac and "qorka_pc.py" for Windows. You will see the code file is divided into three distinct parts called the "Arenas".

![alt tag](http://2.bp.blogspot.com/-ugHM0kKYpiI/VZu_pljBmbI/AAAAAAAAB9g/CF3k5swL1ac/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.28.13%2BPM.png)

The first arena is where you can import different libraries and use different APIs specific to python language. The default imports consist of date and time. All imports happen in a list. The following are some dummy lists, they are for understanding of the layout.

![alt tag](http://1.bp.blogspot.com/-i2PXETWmF08/VZu_p85oPtI/AAAAAAAAB9k/gg-efHy53co/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.27.54%2BPM.png)

The second arena is the place where all the functions are defined. The functions are defined in the 'Function Block'. The default functions given are 'add', 'multi', 'div' and 'sub'. You can add your own functions while creating your own programming language.

![alt tag](http://3.bp.blogspot.com/-ZrE2Bf_QpH4/VZu9mK0nHsI/AAAAAAAAB80/23UH6ED9P7c/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.21.51%2BPM.png)

The third arena is made of two parts. The UI code (which we do not need to alter) and The Execution code. 
The UI code consists of the UI that you see the first time you open Qorka.

![alt tag](http://3.bp.blogspot.com/-ifjlpb3L4D8/VZu9mw_R82I/AAAAAAAAB9A/gF_Kja85mUw/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.21.58%2BPM.png)

The Execution code is the main playground. It is tailored to function as the basic Qorka interpreter.

![alt tag](http://4.bp.blogspot.com/-tnQLgJURNvo/VZu9nlx9qZI/AAAAAAAAB9U/k9p9z5MQx8g/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.22.07%2BPM.png)

Qorka : Getting started
=======
Lets say you want to build a programming language (code interpreter), the first thing you need to add is a "print" function. 

Playing : First arena
--------------
For this simple operation we do not need to import any modules into the first arena. So we leave the first arena as is.

Explaining : Second arena
--------------
Jumping to the second arena, we now need to explain Qorka about what a print function is and what it will do. So we quickly define a print function. I will name my function as gab! (This means each time I enter "gab Hello, World." the program will print the text after gab.

![alt tag](http://2.bp.blogspot.com/-HVNfZmmHTk8/VZvO63gGpGI/AAAAAAAAB94/fyV-Ndf1d8s/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.57.43%2BPM.png)

Executing : Third arena
--------------
Here you need to define exactly when do you want the function to execute. We want the function to execute each time the word "gab" is found in the codeline.

![alt tag](http://1.bp.blogspot.com/-fl0ewZP6c1c/VZvO7P-T0wI/AAAAAAAAB98/2DuretayVkA/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.58.46%2BPM.png)

Saving your Qorka program
--------------
Once you're done with all the three arenas, save the code as "qorka_mac.py" to your desktop.

Operating in your programming language
--------------
By saving the Qorka file, you have now created your programming language (code interpreter). Now let us write a simple "Hello, World." program using your programming language.

![alt tag](http://3.bp.blogspot.com/-cEN3TyOmonE/VZvO7CZwL8I/AAAAAAAAB-A/NYKyLQSiBpM/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B6.05.06%2BPM.png)

Open up a text editor, and write down "gab Hello, World".
Now save the file as "MyProgram.txt" on your Desktop.

Executing the code
--------------
Congratulations you have successfully created your own programming language (code interpreter) and have also written down your first Hello, World. code in your own programming language (code interpreter). Now we just need to run it, and see how things go! To do so, first make sure you have two files posted on your desktop.
- MyProgram.txt
- qorka_mac.py or qorka_pc.py

Now open up the terminal on Mac or command prompt on Windows, and change the directory to Desktop. Use the following command to do so:
> cd desktop

![alt tag](http://1.bp.blogspot.com/-ZQEUp2Vklqc/VZwStZ1wuXI/AAAAAAAAB_M/hApaBXN_8N8/s1600/1.png)

Now, run the Qorka python file. To do so, input the following command:
> Python qorka_mac.py

![alt tag](http://1.bp.blogspot.com/--NJlLKwXW8c/VZwStiHl6AI/AAAAAAAAB_U/0nnh0SUZazw/s1600/2.png)

Once you hit enter, Qorka will ask you for the location of your code (that is MyProgram.txt).

![alt tag](http://3.bp.blogspot.com/-9cSWKwbrU0Y/VZwStouzsLI/AAAAAAAAB_Q/WlTO4YILprU/s1600/3.png)

Once you enter the MyProgram.txt file location, your code will run on the programming language (code interpreter) you have created. And you will see the output at follows.

![alt tag](http://3.bp.blogspot.com/-zDZwzK2DTm0/VZwSum3OfjI/AAAAAAAAB_k/5nXkB_kmOWY/s1600/4.png)

What's more?
--------------
This way you can create n number of functions and define n number of operations to create a language that does more than just saying "hello". Check this out, my language also incorporates math functions, commenting facility, and much much more. Check this out, here is my new set of code lines.

![alt tag](http://1.bp.blogspot.com/-uLZfvSPNTgY/VZwSu9u22oI/AAAAAAAAB_s/CPVCUjX39e0/s1600/5.png)

And here is how it functions!

![alt tag](http://2.bp.blogspot.com/-uyanMAsNLeM/VZwSvB7EMyI/AAAAAAAAB_o/E3iUTo5jvGQ/s1600/6.png)

You can also make a programming language (code interpreter) that operates in your mother tongue. This will allow anyone using your progrmming language to code in your local language. For example, let  us set up a coding environment in Hindi (national language of India).

Programming in Hindi and other local languages
--------------
We use the same process of defining a function in the second arena and executing it in the third arena. Only this time we use Hindi characters so that people can code in Hindi. "Print" in Hindi is called "छाप"(read as chapp). We will use this in Qorka to define a print function.

![alt tag](http://1.bp.blogspot.com/-ioukixkkhDE/VZxX7SKiCaI/AAAAAAAACAg/mXu8loQPDIU/s1600/Screen%2BShot%2B2015-07-08%2Bat%2B4.20.32%2BAM.png)

First define the "chapp" function in the first arena.

![alt tag](http://1.bp.blogspot.com/-D42wkrydAFY/VZxX7TClEDI/AAAAAAAACAY/Iul9kOyIvD4/s1600/Screen%2BShot%2B2015-07-08%2Bat%2B4.20.42%2BAM.png)

After that, write the code of execution in the second arena.

![alt tag](http://2.bp.blogspot.com/-RM5CS4Tfa7Y/VZxX7Qob88I/AAAAAAAACAc/sgNDXC13aSk/s1600/Screen%2BShot%2B2015-07-08%2Bat%2B4.20.19%2BAM.png)

And finally, write it down in the code lines file.

Qorka : Program information
=======
Here is some quick information about Qorka and its build.
- Program name : [Qorka](http://qorka.sourcenet.in)
- Program description : This is Qorka. A python interface for developers to easily create and execute simple interpreters that allow simulation of simple programs.
- Program version : 1.0
- Supporting OS : Mac OSX & Windows
- Created by : [Nirman Dave](http://www.nirmandave.com)
- Licensed to : [SourceNet.in](http://www.sourcenet.in)
- Website : [qorka.sourcenet.in](http://qorka.sourcenet.in)
- Built on : Python 2.7.6 (Pre-Requisite for Qorka)

Qorka : Copyright notice, terms & conditions
=======
(c) Copyrights 2015 by [Nirman Dave](http://www.nirmandave.com). All rights reserved.

This work may be modified, reproduced, distributed, performed, and displayed for any purpose but must acknowledge "[Nirman Dave](http://www.nirmandave.com)", "[SourceNet](http://www.sourcenet.in)" and "[Qorka](http://qorka.sourcenet.in)". Copyright is retained and must be preserved. The work is provided as is; no warranty is provided, and users accept all the liability.
