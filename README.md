cas_network_login
=================

A python and Linux like shell . For the login system of UCAS .

Note!!
---------
This program authored by Zhu Jinliang original.
Edited by me for the Gentoo Linux System.


Edited
---------------
For Gentoo Users, Please Note that , this is for Python 2.7.
If you have installed python 3.2 or higher.

'emerge virtualenv'

choose a folder then 'mkdir virtualenv-app'

then 'su' , 'eselect python list'

You will see a list like this :
   Available Python interpreters:
   [1]python2.7
   [2]python3.2 *

'eselect python set 1'
'etc-update && env-update && source /etc/profile'
'cd virtualenv-app && virtualenv cas'
then copy the program into the cas folder
'source ./virtualenv-app/cas/bin/active'
You will see a new bash like this:
"(cas)nf@wii ~/Apps/virtualenv-app/cas/bin $  "
then run the program 
'python cas_login.py 3'
then fix the system python version to 3.2
'eselect python set 2'
'etc-update && env-update && source /etc/profile'

Contact Me
--------------
Contact Me: zzhhgo#gmail.com

Original README CONTENT
----------------------
----------------------

Overview:
---------
This script is for UCAS student to login the network in Chinese Academy
of Sciences.

若第一次使用，注意先在user_data中的username和password中修改自己的信息。

How to use:
----------
Run it like:
python cas_login.py [option]
You can only input one option.
Options are as follows:
0: 登出
1: 连接城域
2: 连接国内
3: 连接国际

For example: 
When you want to connect to international, input this:
python cas_login.py 3
When you want to logout, input this:
python cas_login.py 0


Note:
-------
Since the author's ability is limited, the software may exist many bugs
that I didn't have found and solve them. Please write them in a file, 
and send to me if possible. I'll appreciate your work very much!

Contact:
---------
If you want to make contact with me, mail me at this:
zhujinlianghust#gmail.com

-Zhu Jinliang, Dec 2012
