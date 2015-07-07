Qorka
=======

![alt tag](http://3.bp.blogspot.com/-Jq-LXLknT-o/VZu1kXSJS3I/AAAAAAAAB7o/kd-Qy4_eKeA/s1600/mac-book-air-2%2Bcopy.png)

Qorka is an interpreter development platform from SourceNet which allows you to creatively put together your own programming interpreter with ease. This means that I can create my own programming syntax, by defining each fucntion on the Qorka platform. And everytime I write a program with my own programming syntax (programming laguage) in a text editor and run it on Qorka, it will execute the file code according to the functions defined by you.

The Qorka environment
=======

![alt tag](http://2.bp.blogspot.com/-rCPA4VoA3Oc/VZu7e23nhUI/AAAAAAAAB8o/u3t4LKZUtC8/s1600/summer%2Bjam%2Bseries.jpg)

Qorka is completely written in python. To get started, first open the Qorka code file, "qorka_mac.py" for Mac and "qorka_pc.py" for Windows. You will see the code file is divided into three distinct parts called the "Arenas".

![alt tag](http://2.bp.blogspot.com/-ugHM0kKYpiI/VZu_pljBmbI/AAAAAAAAB9g/CF3k5swL1ac/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.28.13%2BPM.png)

The first arena is where you can import different liberaries and use different APIs specific to python language. The default imports consist of date and time. All imports happen in a list. The following are some dummy lists, they are for understanding of the layout.

![alt tag](http://1.bp.blogspot.com/-i2PXETWmF08/VZu_p85oPtI/AAAAAAAAB9k/gg-efHy53co/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.27.54%2BPM.png)

The second arena is the place where all the functions are defined. The functions are defined in the 'Function Block'. The default functions given are 'add', 'multi', 'div' and 'sub'. You can add your own functions while creating your own programming language.

![alt tag](http://3.bp.blogspot.com/-ZrE2Bf_QpH4/VZu9mK0nHsI/AAAAAAAAB80/23UH6ED9P7c/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.21.51%2BPM.png)

The third arena is made of two parts. The UI code (which we do not need to alter) and The Execution code. 
The UI code consists of the UI that you see the first time you open Qorka.

![alt tag](http://3.bp.blogspot.com/-ifjlpb3L4D8/VZu9mw_R82I/AAAAAAAAB9A/gF_Kja85mUw/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.21.58%2BPM.png)

The Execution code is the main playground. It is tailored to function as the basic Qorka interpreter.

![alt tag](http://4.bp.blogspot.com/-tnQLgJURNvo/VZu9nlx9qZI/AAAAAAAAB9U/k9p9z5MQx8g/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.22.07%2BPM.png)

Building an interpreter with Qorka
=======
