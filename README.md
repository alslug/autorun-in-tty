# autorun-in-tty
How do you have a specific program run in a tty on your linux-box?

Easy. Place these files in a folder named

* /etc/systemd/system/getty@tty1.service.d
* /etc/systemd/system/getty@tty2.service.d
* /etc/systemd/system/getty@tty3.service.d
* etc

to get the program running in the specific tty (you normally get to them using Ctrl-Alt-F1 / Ctrl-Alt-F2 etc )

If you what the tty to clear after each exit skip the noclear.conf file.
