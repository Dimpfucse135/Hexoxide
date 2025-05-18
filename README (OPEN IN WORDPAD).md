  ___ ___                            .__    .___      
 /   |   \   ____ ___  __________  __|__| __| _/____  
/    ~    \_/ __ \\  \/  /  _ \  \/  /  |/ __ |/ __ \ 
\    Y    /\  ___/ >    <  <_> >    <|  / /_/ \  ___/ 
 \___|_  /  \___  >__/\_ \____/__/\_ \__\____ |\___  >
       \/       \/      \/          \/       \/    \/ 

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Hexoxide is a GDI Trojan.
Written in C++, may it's name look promising, but it isn't!
This malware consists of demo-esque visuals (using GDI), ear-tearing music (bytebeats, an audio making program), the salvia divinorum shall the computer take, and the way it shatters your PC apart.
The malware took me 4 days to make, vice-versa, and all the eye candy.
There are 4 versions of this malware with different behaving variants, as it says in the title.
The versions of this malware are:

[-----------------------]
[HexoxideROWSAFETY]
[HexoxideROWDESTRUCTIVE]
[Hexoxide (itself)]
[HexoxideSAFETY]
[-----------------------]

------------------------------------------------------------------------------------

___________              .__                        __  .__               
\_   _____/__  _________ |  | _____    ____ _____ _/  |_|__| ____   ____  
 |    __)_\  \/  /\____ \|  | \__  \  /    \\__  \\   __\  |/  _ \ /    \ 
 |        \>    < |  |_> >  |__/ __ \|   |  \/ __ \|  | |  (  <_> )   |  \
/_______  /__/\_ \|   __/|____(____  /___|  (____  /__| |__|\____/|___|  /
        \/      \/|__|             \/     \/     \/                    \/ 

------------------------------------------------------------------------------------

The way hexoxide makes visuals, is through an API called GDI (Graphics Device Interface), using Blt (StretchBlt, BitBlt, PatBlt, etc.).
Before that, you need a variable called "HDC", HDC is an integer, containing the screen.
Then, it uses that HDC for the Blts, and it would work, but you need the screen width and height portions too.
To get the screen boundaries, we will have to use a function called "GetSystemMetrics".
This is how i made the GDI, lets move on to the bytebeat.

The bytebeat is pretty simple to go through.
Basically it uses a formula to change a variable called "t", and then it makes a 32 bit audio to play the formula.
