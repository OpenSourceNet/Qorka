Qorka
=======

![alt tag](http://3.bp.blogspot.com/-Jq-LXLknT-o/VZu1kXSJS3I/AAAAAAAAB7o/kd-Qy4_eKeA/s1600/mac-book-air-2%2Bcopy.png)

Qorka is an interpreter development platform from SourceNet which allows you to creatively put together your own programming interpreter with ease. This means that I can create my own programming syntax, by defining each fucntion on the Qorka platform. And everytime I write a program with my own programming syntax (programming laguage) in a text editor and run it on Qorka, it will execute the file code according to the functions defined by you.

The Qorka environment
=======

![alt tag](http://2.bp.blogspot.com/-rCPA4VoA3Oc/VZu7e23nhUI/AAAAAAAAB8o/u3t4LKZUtC8/s1600/summer%2Bjam%2Bseries.jpg)

Qorka is completely written in python. To get started, first open the Qorka code file, "qorka_mac.py" for Mac and "qorka_pc.py" for Windows. You will see the code file is divided into three distinct parts called the "Arenas".

![alt tag](http://3.bp.blogspot.com/-9i_y-YkxF9Q/VZu6xoxRPqI/AAAAAAAAB8I/WoGa51vL91Y/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B4.59.57%2BPM.png)

The first arena is where you can import different liberaries and use different APIs specific to python language. The default imports consist of date and time. All imports happen in a list. The following are some dummy lists, they are for understanding of the layout.

![alt tag](http://1.bp.blogspot.com/-F_YF730Wqbo/VZu6xqkYzCI/AAAAAAAAB8E/xOB0hr_wEq4/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.02.45%2BPM.png)

The second arena is the place where all the functions are defined. The functions are defined in the 'Function Block'. The default functions given are 'add', 'multi', 'div' and 'sub'. You can add your own functions while creating your own programming language.

->![alt tag](http://3.bp.blogspot.com/-gyec18bvEEI/VZu6xKYLzVI/AAAAAAAAB8A/FY-_mUNzCVg/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.04.59%2BPM.png)<-

The third arena is made of two parts. The UI code (which we do not need to alter) and The Execution code. 
The UI code consists of the UI that you see the first time you open Qorka.

![alt tag](http://3.bp.blogspot.com/-iy7NRPAYQXE/VZu6yf6rZ-I/AAAAAAAAB8Q/g1gXQGj2XAE/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.07.57%2BPM.png)

The Execution code is the main playground. It is tailored to function as the basic Qorka interpreter.

![alt tag](http://4.bp.blogspot.com/--GAhYagLf-0/VZu6y_mia0I/AAAAAAAAB8c/EtZSCNjuVYw/s1600/Screen%2BShot%2B2015-07-07%2Bat%2B5.08.15%2BPM.png)

Building an interpreter with Qorka
=======
