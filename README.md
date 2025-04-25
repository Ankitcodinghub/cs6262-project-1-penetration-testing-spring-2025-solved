# cs6262-project-1-penetration-testing-spring-2025-solved



**<span style='color:red'>TO GET THIS SOLUTION VISIT:</span>** https://www.ankitcodinghub.com/product/cs6262-project-1-introduction-to-penetration-testing-spring-2025-solved/

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;127366&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;5&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (5 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS6262 Project 1-Penetration Testing Spring 2025 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">
            
<div class="kksr-stars">
    
<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
    
<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>
                

<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (5 votes)    </div>
    </div>
The goal of this project:

Penetration testing is an important part of ensuring the security of a system. This project introduces some of the common tools used in penetration testing, while also exploring common vulnerabilities (such as Shellshock and setUID bit exploits).

On September 24, 2014, a severe vulnerability in Bash, nicknamed Shellshock, was identified. This vulnerability can exploit many systems and be launched either remotely or from a local machine. In this project, you will gain a better understanding of the Shellshock vulnerability by exploiting it to attack a machine. The learning objective of this project is to get first-hand experience on this interesting attack, understand how it works, and think about the lessons that we can get out of this attack.

Environment Setup:

Files Provided Description

shellshock_server.ova The VM image.

assignment_questionnaire.txt Template for final submission.

This project requires the use of virtual box and multiple VMs.

Installing Virtual Box:

1. Install VirtualBox if it is not already installed. This project requires the latest version of VirtualBox. Using an earlier version of Virtual Box has been known to cause errors where the project VM freezes, so if you run into this, ensure you are running on at least Virtual Box 6.1.0 or later.

2. Download the Oracle Virtual Box Extension Pack (available for download at the same location as Virtual Box is).

3. Import the Extension Pack under File-&gt; Tools -&gt; Extension Pack Manager

4. In Virtual Box go to File -&gt; Tools -&gt; Network Manager

5. Select the NAT network tab and click on Create. Right click on the newly created NAT network, click on Properties and rename it to something related to the project. Then save it and close the preferences.

Installing the Kali Linux VM (feel free to use any other OS but we recommend using Kali):

6. Download the 64bit VirtualBox version of the Kali VM from the link: kali download.

7. Extract the above zip and double click on the vbox file. Once you have imported the VM, you’ll need to go into the VM Settings and increase the number of CPUs if possible, as well as the RAM. Also enable 3-d acceleration and set the zoom level to 300 (it makes it easier to read).

8. Go to the new Kali VM’s settings. In the network tab change “Attached to:” from NAT to “NAT Network” in the Adapter 1 tab. The name of the network should autofill to your newly created network if you only have one, but if you have multiple NAT networks, you’ll need to select the correct one.

9. Start the Kali VM. The default username/password is kali/kali.

10. Repeat the process with the other VM (shellshock_server.ova) which you will download in a later step so that these two VMs can communicate with each other.

Vulnerable machine:

11. Download the project appliance using the link below:

1. shellshock_server.ova sha256sum: b8729307ad6849d17c6b88e8a5893d5f7a7ccf3167d9279e4067039379be1703

12. Double click the downloaded ova file to start its import process.

13. Once imported, adjust the CPU and RAM for this VM like you did for the Kali VM. Ensure Adapter 1 is set to NAT Network and the name of the NAT Network is the name you specified when creating the NAT Network in step 5.

14. Boot up the shellshock_server and you’re good to go.

NOTE: You do not need to into the shellshock VM. Once you see the login screen, you’re good to go.

Leave the shellshock VM running and switch to the Kali VM for the rest of the project now.

15. Now try to connect to the shellshock VM server from Kali. Once you find the IP of the VM in Task 1 below, navigate to the following URL: http://:/cgi-bin/shellshock.cgi Then you should be able to see the content:

16. Notice that you do not need the password to access the web content hosted on the VM server. Instead of using a real server, it is safer to perform the attack on an emulated Apache HTTP Server VM. To be clear, you will not be logging into the shellshock VM during this project. Once you configure the shellshock VM (by following steps 17-20 above), you will be exploiting it externally, from the Kali VM, by exploiting the Shellshock vulnerability.

Project Tasks (100 points):

Task 1: Network Scanning – (10 points)

The first step in any penetration test is to gather information about the network and servers you’ll be exploiting. In this task, you will perform network scanning and answer a few questions based on your findings. On startup, the shellshock VM listens to several ports for incoming messages.

1. Find the IP address of the vulnerable VM on the NAT network using nmap.

2. Use nmap to identify all the open ports on the shellshock server and submit the port number which handles the http traffic to the Apache web server on the VM.

Note: If possible, please use VirtualBox for this part since in the previous semesters VMware has been known to cause some issues with the network setup and Task 1.

Task 2: Attack CGI Program– (20 points)

In this task, you will launch the Shellshock attack on a remote web server. Many web servers enable CGI, which is a standard method used to generate dynamic content on Web pages and Web applications. Many CGI programs are written using a shell script. Therefore, before a CGI program is executed, the shell program will be invoked first, and such an invocation can be triggered by a user from a remote computer.

To access this CGI program from the Web, you need to first check the server VM is running. Then, you can either use a browser by typing the following URL:

http://:/cgi-bin/shellshock.cgi

or use the following command line program curl to do the same thing:

$ curl http:// :/cgi-bin/shellshock.cgi

For this task, your goal is to launch the attack through this URL, such that you can achieve something that you cannot do as a remote user. For example, you can execute some file on the server, or look up some file located on the server. When you successfully launch an attack, please execute the /bin/task2 program (which needs your GT username as the input) inside the VM. It will generate the submission hash for you.

For students that want to verify their work, here’s an example correct input/output for /bin/task2:

$ /bin/task2 gburdell3 Here is your task2 hash:

5732307cf1ef49dd2613e9bbe28dd3e0ea907c28d6c8736faf0c9537c2b20c5a

Task 3: Reverse Shell with Metasploit – (25 points)

Now you have successfully launched the Shellshock attack, and you can execute commands on the server VM. However, during a penetration test, you likely won’t have time to craft a payload for every exploit you use. And, what if the server was not in fact vulnerable to shellshock. How would you know if your exploit failed because it was wrong, or because there was not a vulnerability?

That is where Metasploit comes in. Metasploit is a standard in the penetration testing community. It allows pen testers to run precompiled exploits against a host, using predefined payloads. For this project, we’re going to use Metasploit to establish a reverse shell between your machine and the host machine.

Let us first see how Metasploit works by using it to scan the open TCP ports of the shellshock_server VM. While this is a task better suited to tools like nmap (as seen in Task 1), it serves as a good demonstration of how to use a Metasploit module. If you have used Metasploit before, you can skip this introduction and go directly to the Task 3 assignments section at the end.

msfconsole

1. Begin by opening a new terminal on your Kali VM. In the new terminal type: . After a moment, the Metasploit Framework console (msfconsole) will load. For this project, the msfconsole is the main way of accessing Metasploit. While there are other tools and command prompts associated with Metasploit, the msfconsole is suitable for the entirety of this project.

2. For this example, we’re going to scan the ports of a host. You can use the results from task 1 to ensure Metasploit is behaving properly. In practice using a Metasploit module solely for the purpose of scanning ports on a host is a little overcomplicated, since nmap can do much more and takes less setup, but this does offer a good introduction to using a Metasploit module.

3. A metasploit module is the base of any task performed in metasploit. It consists of Ruby code that is written to perform a certain task (like exploiting a certain vulnerability or scanning a certain kind of system). There are multiple different varieties of modules, but for our purposes we’ll focus on three of them:

a. The Exploit modules: These are modules written to exploit a certain vulnerability.

b. The Auxiliary modules: These are modules written to perform some tasks related to exploiting a system (like scanning). Within the auxiliary modules there are many kinds of modules. We’ll be using the “scanner” modules for this example.

c. Payloads: Calling these modules is a little misleading. They are the payloads (for example the shellcode) that are sent within the exploit.

The reason there are so many results is that “scanner” is a class of auxiliary modules (as seen by there being so many modules beginning with “auxiliary/scanner”). So, searching for “scanner” (or “scan”) will give everything at all related to network or vulnerability scanning.

That seems a little better. Only 7 results. Since we’re scanning for open tcp ports, let’s use: “auxiliary/scanner/portscan/tcp”. To use a metasploit module, you should run the command: use module_name

You should now see “auxiliary(scanner/portscan/tcp)” after “msf5” indicating you are using the auxiliary(scanner/portscan/tcp) module.

6. Now that we’re using the correct module, we must set the correct options. Try running the

command options . You should see something like:

While each of the options is marked as required, most of the pre-filled values work for our purposes. The only one we need to change is RHOSTS. RHOSTS should be the IP address of the host we want to scan. In this case, you should set it to the IP address of the shellshock_server VM, that you found in part 1. You can use the command: set rhosts IP_of_host. Now try running options again and ensure the RHOST option is set to the right IP address.

Now run run and you should see the same list of open ports that nmap showed. While “run” is

usually used to run auxiliary exploits, the command “check” and “exploit” are often used to check

7.

and run exploit modules.

Now you’ve seen an example of how to use Metasploit. You’ll follow a similar process when exploiting the shellshock vulnerability.

Task 3 Assignments:

1. Find an exploit module that exploits the shellshock vulnerability on an Apache web server. Once you’ve found the module, place the module name in assignment_questionnaire.txt.

2. Use show payloads to show the possible payloads for the module. Find a payload that spawns a reverse tcp shell. Place the full name of the payload in assignment_questionnaire.txt.

3. Run the exploit and spawn a reverse shell on the VM.

4. Run /bin/task3 in the resulting shell, then type cs6262 then your user ID. Report the hash value for your user ID in assignment_questionnaire.txt.

You’ll submit all your answers for this section in assignment_questionnaire.txt. You should keep the reverse shell running after finishing Task 3, as you will need it in Task 4.

Task 4: Privilege Escalation – (20 points)

Your goal:

You aim to upgrade the privilege for your command shell by exploiting the setUID vulnerability. You will run /bin/task4 as the higher privileged user “shellshock_server”, not the default user “www-data”.

Background:

In Unix based systems, setUID is access rights flags that determine what users can run a program. For

instance, when users want to change their password, they may run the passwd that requires root privilege. The setUID can help the user run the passwd with temporarily elevated privileges. However, if setUID is misused or setUID flags are misconfigured, it can cause a variety of vulnerabilities such as information leakage, unwanted privilege escalation, etc.

Assignments: in your shell. You should see “www-data” which is your user ID. Now, run

As a first step, type whoami

/bin/task4 gt_usernam

e. You would see a permission denied error. That is because /bin/task4 is

configured to allow only the “shellshock_server” user to run it. So, you need to find a way to run task4 as the “shellshock_server” user. A feasible approach is to spawn a shell running as a “shellshock_server” user and run task4 through it.

Your goal is to find a program which:

1. Has a higher privilege than the default user.

2. Can spawn a shell.

Useful Resource: https://gtfobins.github.io/

You may want to ransack /usr/bin for a program which has a higher privilege than the default user and run /bin/task4 gt_username in the shell spawned.

What is the vulnerable program? What command do you use to search it? What command do you use to spawn a shell with the vulnerable program? And what is the hash value from /bin/task4 gt_username (like /bin/task2)? Please leave your answers in assignment_questionnaire.txt.

NOTE: If you exploit a symlinked binary, submit the name of the target binary that is linked. Eg: If binary A points to binary B, submit binary B as the answer.

Task 5: Password Cracking – (25 points)

An invaluable part of any penetration test is password cracking. While there may be no known vulnerabilities in a system, a weak password could be just as damaging in allowing an attacker to gain access to a system (or view sensitive information once they gain access). We’re going to look at two kinds of weak passwords in this task: passwords that are too short, and passwords that can easily be guessed via password scraping.

To begin, start a Meterpreter shell (using a meterpreter shell payload) through the Metasploit shellshock module in Task 3. A Meterpreter shell is different from the reverse TCP shell in Task 3, as it allows you to run Metasploit specific commands on the vulnerable machine (like download). Navigate to

/home/shellshock_server/secret_files/. There are two encrypted .pyc files here. task51.zip is encrypted with zip, while task52.pyc.gpg is encrypted with gpg (a common file encryption tool in Linux). Download these two files (task51.zip and task52.pyc.gpg) to your Kali VM using the meterpreter.

We already know the developers of this web server are not very security savvy, since they let a shellshock vulnerability plus a setUID exploit give a high privilege shell on their machine. So, chances are they did not pick very secure passwords for these secret files. Your goal in this task is to crack the passwords of these two files using John the Ripper (a popular password cracker) and cewl (a password scraper).

The command line tools used in Task 5 are in /usr/sbin on the Kali VM. To run them, you can either add /usr/sbin to the $PATH variable or write /usr/sbin/ before each command.

You should use zip2john and gpg2john to extract the password hashes from the encrypted files. For task51.zip, try running John the Ripper incrementally. Report your John the Ripper command in assignment_questionnaire.txt (whether you also report your the zip2john and gpg2john commands is up to you, but they will not be graded).

For task52.pyc.gpg, try running John the Ripper incrementally again. Hmm… it seems to run forever. That is because John the Ripper is trying every combination of characters. If the password is too long (among other things), John the Ripper could run for years before it finds it.

Just because the password is too long to be found incrementally, does not mean it cannot be cracked. Take a look at the shellshock.cgi page in the browser. It looks like it gives a link to a profile of the authors. If the authors are not great at picking secure passwords, maybe the password is something about them that we can guess from their profile page.

But, even if the password is on the profile page, it can still take a while to guess by hand. What if the password was kItt3n$ or deVEL0p3r. It would be hard to guess that, even if the word it was based on (like “kittens”, or “developer”) was on the profile page.

Instead, let us use a password scraper to create a custom wordlist for John the Ripper. For this project, we suggest using cewl. cewl is a simple command line program that comes preinstalled on Kali and creates password word lists off of webpages. Since we want to get every possible password (including if the authors based the password off something on shellshock.cgi, or one of the landing pages), you should run cewl on shellshock.cgi, with the proper settings to ensure it follows the links all the way to profile.cgi (you may need to tune the cewl parameters). Report your cewl command in assignment_questionnaire.txt. Then try running John the Ripper on task52.pyc.gpg with the wordlist (and the default wordlist rules for testing different permutations of the words). Report your John the Ripper command in assignment_questionnaire.txt.

Once you find the passwords, report them in assignment_questionnaire.txt. Then decrypt the two files (using zip for task51.zip and gpg for task52.pyc.gpg) and run python2.7 task51.pyc gt_username and python2.7 task52.pyc gt_username. Report the resulting hash values for your user ID in assignment_questionnaire.txt.

Deliverables:

Please use Gradescope to submit the assignment files. The link to Gradescope is found in Canvas under Courses tab -&gt; Gradescope. In Gradescope under active assignments click project 1 to upload your files.

● assignment_questionnaire.txt

● README.txt

The provided template “assignment_questionnaire.txt” marks where you should add your answers for each question. Please DO NOT edit anything other than the fields marked for your answers (or student ID) in assignment_questionnaire.txt. Doing so may result in the autograder failing to process your submission.

Please note that there is a 5-point penalty for not following the format given in assignment_questionnaire.txt.

You should also include a “README” plain text file explaining how and why each piece of your solution works. Including it makes grading easier if we cannot reproduce your results. You may also include screenshots in your submission to show proof. To include screenshots (optional), upload them to your GT SharePoint drive and add a link in the README.txt file. If you use any outside sources not mentioned in this write-up, then README would be a good place to mention them as well. The README.txt file is a plain text file, and no other formats are accepted.

FAQ:

● For this project, students have unlimited submissions on gradescope.

● You do not need to log into the shellshock image at any point to complete this project.

● For all task binaries, make sure to pass in your GT Username as the argument (e.g.: gburdell3) and beware of extra spaces after your name because that will result in an incorrect hash.

● Make sure you are using atleast VirtualBox 6.1.x. (students have completed the project on other versions too, but it sometimes causes issues).

● Make sure to assign at least 2 CPUs and 4GB of RAM to your shellshock image for it to function properly.

● The objective of this project is to get you familiarized with the absolute basics of penetration testing and therefore we encourage Googling to learn more about the vulnerability, the tools, and the attack concepts.

Reminders:

Please submit the files EXACTLY as requested to Canvas. DO NOT package them up (e.g., as a ZIP file). Any deviations may result in a deduction of your grade.

There is a 5-point penalty for not following the submission format shown.

Useful Links and References:

● Shellshock Vulnerability

◦ https://github.com/carter-yagemann/ShellShock

◦ https://en.wikipedia.org/wiki/Shellshock_(software_bug)

◦ http://seclists.org/oss-sec/2014/q3/650 ● curl

◦ https://curl.haxx.se/docs/manpage.html

◦ https://curl.haxx.se/download.html (curl.exe for Windows) ● netcat

◦ https://linux.die.net/man/1/nc

◦ https://eternallybored.org/misc/netcat/ (nc.exe for Windows)

● nmap

◦ https://nmap.org/book/man.html

◦ Service and Version Detection | Nmap Network Scanning ● Metasploit

◦ https://www.offensive-security.com/metasploit-unleashed/metasploit-fundamentals/

● John the Ripper

◦ https://www.openwall.com/john/doc/ ● cewl

◦ https://tools.kali.org/password-attacks/cewl

Acknowledgment:

This Lab was modified from SEED Labs, Copyright 2014 Wenliang Du, under the terms of GNU Free

Documentation License, Version 1.2. The original document can be found at http://www.cis.syr.edu/~wedu/seed/

Checklist/Rubric:

Section Points ✓

1 Network Exploration 10

1.1 Correct first digits of the IP Address of the vulnerable VM. 5

1.2 Correct HTTP port. 5

2 Exploiting the System 20

.

1 Command used to exploit the shellshock vulnerability. 5

2.2 Correct hash value from running /bin/task2. 15

3 Spawning a Shell with Metasploit 25

3.1 Correct exploit module 5

3.2 Correct payload module (there are multiple correct answers here) 5

3.3 Correct hash value from running /bin/task3. 15

4 Privilege Escalation 20

4.2 Correct vulnerable program name. 10

4.4 Correct hash value from running /bin/task4 10

5 Password Cracking 25

5.2 Correct password for task51.zip. 5

5.3 Correct hash value from running python task51.pyc. 7.5

5.6 Correct password for task52.pyc.gpg. 5

5.7 Correct hash value from running python task52.pyc. 7.5

– Possible Deductions

i. Incorrect assignment_questionnaire.txt format. -5

ii. Incorrect upload to Gradescope/Canvas. -5

+ Your Submission Includes Total: 100

assignment_questionnaire.txt – Answers to questions

README.txt
