# Sprak_FakeDOS
FakeDOS operating system for Else Heart.Break() computer terminals

# Files:
  * Binary.spk : Implementation of a ASM interpreter for the FakeDOS OS. Still on very early alpha.
  * Editor.spk : File editor for the machine. You can grab this if you don't want the OS, just the editor.
  * FakeDOS+Editor.spk: The OS with the Editor. This is the working version of the OS. You should grab this.
  * FakeOS_With_Editor+smallFakeASM.spk : The full version. Not working at the moment (needs jsut some tweaks to make it run). Includes the ASM thing.
  * HexView.spk : A hex viewer for the ASM files.
  * FakeASM_doc.txt : Description of the FakeASM language, in txt format
  * smallFakeASM_doc.pdf : Description of the FakeASM language, in pdf format
  
 TLDR: Just get the FakeDOS+Editor.spk file.
  


# How to use:
Pick a computer in the game that has a big screen (best for the editor. I recommend the one in the basement of the Hotel.)
Hack a screwdriver, and change the code to 
```lua
SetMhz(500)
EnableAPI("floppy")
EnableAPI("memory")
```
Now use the screwdriver on the computer.
Now hack the computer and copy the code to the machine.

# FakeDOS first use:
FakeDOS searches in the computer memory for its partition table. If it doesn't find it, it tells you to format the computer.
In your first use, you'll need to format it. (I'll erase the computer memory!)
In the first run, use "sys c:" to format it. If you type any other command, it'll hang the computer, so you need to reboot it.

# FakeDOS commands
After formatted, you can use the basic ol' DOS commands to navigate around:

* DIR - Lists all files and directories inside the current directory
* CLS - Clear Screen
* HELP - Lists avaliable commands
* MD - Create a directory. Ex: "md test_directory"
* CD - Change directory. Ex: "cd test_directory"
* RD - Remove Directory. Ex: "rd test_directory"
* EDIT - Edit files. Ex: "edit test_file"
  
 # FakeDOS ASM
 It was an attempt to create a assembly language for the computer. It has some basic commands, but it is FAR FAR from complete. Consider it a pre-alpha v0.1.
 In the current state it'll not run correctly. If you are not trying to develop this, just use the FakeDOS+Editor.spk file.
