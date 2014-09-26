Sem7-SIL-A0
===========
Project 0 - Starting with the Basics (50 points)

This project will help us setup the infrastructure to do the "real” projects later on. In this project, you will create 2 VMs on your computer. You can use any Virtualization Technology, the instructions I'm providing here assume that you are using VMWare. A minor bit of Googling will show you how to do this with Virtualbox, which is the other popular technology.

Create a VM that runs Kali Linux. You can find a pre built VM at http://www.kali.org/downloads/

Create another VM that runs Metasploitable, which is an image that (intentionally) has known vulnerabilities. You can find it at http://www.offensive-security.com/metasploit-unleashed/Metasploitable

Run metasploit on Kali. It doesn't run by default, and needs Postgres to be running as well. See https://community.rapid7.com/community/metasploit/blog/2013/03/13/metasploit-now-supports-kali-linux-the-evolution-of-backtrack for instructions. Use metasploit to probe the metasploitable VM, using particularly nessus and nexpose. To learn more about Metasploit and how to use it, try http://www.offensive-security.com/metasploit-unleashed/Main_Page.

Once you've identified vulnerabilities, use the exploits available in metasploit to attack at least one of them. Run wireshark and capture all packets corresponding to your attack session.

Make sure that you use the host only networking mode of VMWare (or analogous modes in Virtualbox -- see https://blogs.oracle.com/fatbloke/entry/networking_in_virtualbox1) so that these VMs can see each other (and the host), but NOT see the outside network. This is as much for your own good as that of the rest of the world.

What to Submit (in a single zipped/tarred file):

    A screenshot showing your two VMs running on your host, with a window on each with the output of the uname -a command visible.

    A screenshot showing wireshark with the packet capture of your attack session.
    A 1 page report of what tools you used, what vulnerabilities you found, what exploits you used against them, and with what results. Describe how the wireshark packet capture helped you understand the attack. 
