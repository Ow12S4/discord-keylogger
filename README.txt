Got bored and decided to write up a quick keylogging program that
transmits data back to a Discord server which acts as a C2. 

Instructions:
      1) Login to Discord.com
      2) Click the '+' button on the left-hand navigation bar to
         create a Discord server for free.
      3) Once done, right click the server and select 'Server Settings'
      4) Under the 'Apps' category, select the 'Integrations' tab
      5) Click the 'Webhooks' tab and select 'New Webhook'

The Discord Keylogger in this repository will log up to 1,500 characters
and then dispatch them via HTTP-POST using the Discord Webhook. The logged
keystrokes will end up in whatever #Channel you set your Webhook to post in.

Note: You can increase the size of the character-limit to exceed or stay
below 1,500 characters, however Discord only allows a maximum of 2,000
characters. Keep this in mind.

KNOWN BUGS:
Function keys, hotkeys, and symbols. This is more of a proof-of-concept
script. It is not mean't to be taken seriously and needs serious work to
improve the capture of these specific keystrokes. Symbols often are mixed
up and output isn't very clean. However, Backspaces work and case-Shifts
work perfectly, changing the actual message as the user intended it to be.

TIPS:
Running this script on a Linux/Unix OS require roots elevation. This is
more geared to Windows operating systems. Additionally, using programs
like AutoPyToExe (https://pypi.org/project/auto-py-to-exe/) can be used
to compile Python scripts into Windows Executable files, including the
script dependencies/libraries. This eleminates the need for an interpreter
to be installed on the system.
