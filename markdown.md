# DataSecHW
This is the start of my markdown document for Data Security course of Fall 2022.

h1

Hutchins et al 2011: Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains, chapters Abstract, 3.2 Intrusion Kill Chain and 3.3 Courses of Action, summarized:

The US Department of Defense refers to the Intrusion Kill Chain as a "chain" because it is an integrated, end-to-end process. It consists of C&C, installation, delivery, exploitation, weaponization, and actions on objectives. In order to enter the target environment, intruders must first establish a C2 channel. This enables them to gather, encrypt, and extract data from the victim's environment.
They will then take action to achieve their original goals of data exfiltration and other forms of network intrusion. Figure 2 depicts an example of a seven-month series of intrusion attempts from a single APT campaign.

Debian:

![image](https://user-images.githubusercontent.com/90117364/187293659-9e133f89-4fde-4621-9aea-8f9be903b7bf.png)

  All is good.

Wargames:

  Level 0: 

![image](https://user-images.githubusercontent.com/90117364/187295858-ce161341-50e0-496f-9e15-e909481f752b.png)

  Level 1:

![image](https://user-images.githubusercontent.com/90117364/187297221-103f9737-a235-4aca-9bcc-27690adb90c2.png)

(ok so the first two levels were super simple, besides my general confusion about Debian and PuTTY, but now I kinda understand how terminal-based programs operate.
after that i double-tripple checked the password for the next level but it just kept denying access, i would really like to know why - my best guess is that i'm doing something wrong with my login credentials)

WebGoat 8:

That's what I've had the most confusion with. So in the guide provided on the website, Kali and Ubuntu are used in order to demonstrate the installation process. Thats what really confused me since my Debian VM only has an SSH environment which doesn't recognize "$ sudo" commands. I guess I did something wrong during the installation but everything outside of that seems to work, SSH Wargames for example, not that I tried anything more than that so far.
