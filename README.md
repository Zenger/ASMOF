ASMOF
====

Another Slightly Modified Options Framework

This is a modified version of the <a href="https://github.com/syamilmj/Options-Framework">SMOF</a> but with many many other tricks in it.

<h3>Static Var before global array</h3>
First instead of just using a global array it usses a class to store all your options in a static variable and then it adds them to the global array and populates the field of the ASMOF.
```php
ASMOF::upload('your-id', 'Title', 'Description', 'default value');
ASMOF::section('Section Name');
```
<h3>Restructured defaults logic</h3>
It uses a restructured logic of getting the defaults, it will use your defaults which you have configured at the start and you won't need to make 2 different versions of your settings.
Looks something like this:
```php
ASMOF::get('your-id', 'Optional default value');
```
<h3>Redesigned Layout</h3>
A completely redesigned layout with proper icon setup, you don't have to interefere in Options Framework CSS to add your own icons.

<img src="http://i.imgur.com/tJFjpnV.png" />
<h3>Retina Input</h3>
A modified upload input which allows uploading a simple and a 2x sized image for retina devices, you'll have to work that on the client side on your own ;)
<img src="http://i.imgur.com/Il9Xjvg.png" />

<h3>Errors and Warnings removed</h3>
Removed all warnings and errors that were existing at the time, I've removed a few bugs and changed the code just a little bit. Removed all the old constants and changed them to match new WordPress requirements.

<h3>Portability</h3>
The new code base is portable. Just add 2 constants ADMIN_PATH and ADMIN_DIR. Then move all the directory anywhere you want.

Setup
====
<ol>
<li>Clone ASMOF where you want it to be</li>
<li>Create a configuration file and setup 2 constants. ADMIN_PATH and ADMIN_DIR. Make them point to the folder where Options.php is located</li>
<li>Create your options</li>
</ol>
