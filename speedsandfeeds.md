# Speeds And Feeds

> There is something on my shop network running at nc mercury.picoctf.net 33596, but I can't tell what it is. Can you?

This one starts off with being given an address and a port
Netcat time

Run the command:
nc mercury.picoctf.net 20301 
The ensuing result broke my terminal, but it looks like a lot of Gs followed by
numbers, almost like coordinates. Googling a CNC machine like the hint suggests
that what you're seeing here is G-CODE, what a CNC machine uses to determine
where to cut wood (which is apparently what they do, thanks Hunter, you get
write up credit for educating me)

Running the G-CODE through a simulator (Such as the one below) presents the flag,
which is objectively unique and cool
https://ncviewer.com/


**picoCTF{num3r1cal_c0ntr0l_68a8fe29}**