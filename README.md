# Psion Organiser II programs
These programs were written by me in the late 1980's for my Psion Organiser II XP.  

## LOCK
by Chris Lawrence  

This is a comprehensive security program for any Psion II, which implements a system password, logs incorrect login attempts, and shows contact information in case it gets lost.  

**Instructions**

When run for the first time it will call LOCK$ and prompt for your password (7 chars max) and some information to display (I had a contact number in case I lost my Psion).  Then it will lock your Psion.  

When it is turned on again, you must press ON to proceed - if you don't it simply switches off again after a few seconds.  Once you have pressed ON, it instructs you to press EXE.  If you press EXE, it scrolls the information you entered above and instructs you to press SPACE, upon which it switches off again.  

The idea behind this is that if you lose your Psion, the person will simply be able to view the information and not realise that there is anything else to do.  

Instead of pressing EXE when instructed you should actually enter your password.  If your password is not correct it is stored and the Psion will switch off again.  If the password is correct then you will exit to the main menu.  

If any invalid entries were entered, they will be stored and date/time stamped and you will be warned of these attempts when you enter the correct password.  Simply search your A:MAIN data for the string 'WWX' - this was chosen because it is unlikely to be used for anything legitimate and the keys are handily bunched together near the EXE key.  

The program has full error trapping and checking, and will gracefully deal with any untoward situations like memory becoming low, filesystems not existing, etc.  

**Installation**

Required files:
```
LOCK - main program
LOCK$ - init program (can only be called from LOCK)
```

Type these two programs in, or use the comms link to transfer them from the PC. Translate them, and if you wish save them to a pack. If you are using a 4-line machine, you can translate the procedures normally or with Xtran, as both will produce valid programs.  

Insert LOCK into the main menu (with the Mode key) so that from then on, the L key can be used to lock up the organiser.  

## FILEDIR
by Chris Lawrence  

This is a procedure for the Psion CM/XP that lists all data files in the organiser, including all packs.  

**Instructions**

Simply run the procedure, and press any key whenever you wish to see the next filename.  

**Installation**

Required files:
```
FILEDIR - main program
```

Type in FILEDIR, or use the comms link to transfer it from the PC. Translate it, and if you wish save it to a pack. If you are using a 4-line machine, you can translate this program normally, or with the Xtran option.  

## PACKMEM
by Chris Lawrence  

This is a procedure for the Psion CM/XP that displays the amount of free space on its packs.  

**Instructions**

Simply run the procedure, and press any key whenever you wish to see the next pack. If a pack is found that does not have a MAIN file like it should, it asks if you wish to create it.  

**Installation**

Required files:
```
PACKMEM - main program
YN% - returns 1 if Y is selected in answer to the question supplied
```

Type these two programs in, or use the comms link to transfer them from the PC. Translate them, and if you wish save them to a pack. If you are using a 4-line machine, you can translate the procedures normally or with Xtran, as both will produce valid programs.
