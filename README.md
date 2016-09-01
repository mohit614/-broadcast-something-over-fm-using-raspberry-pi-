# -broadcast-something-over-fm-using-raspberry-pi-               
Broadcast locally, on any particular frequency using Raspberry Pi 2/3                   

Things you must have::->                  

1.A RASPBERRY PI 2/3            
2.A SSH CLIENT TO CONNECT TO RASPBERRY PI USING PC OR LAPTOP e.g. PUTTY for windows                   
3.NOW CONECT TO RASPBERRY PI USING PUTTY                      
4.IF LOGINNG FIRST TIME ....LOGIN ID =pi and PASSWORDS =raspberry                   
5.AFER SUCESSFUL LOGING :               
    A)MAKE A NEW  C FILE (SAY IT my_fm.c)  AND COPY PI_FM.C CONTENT FROM GIT REPOSITORY,  TO THAT FILE  OR SIMPLY CLONE MY GIT REPOSITORY         
            $ sudo nano my_fm.c                                    //PAST  COPIED PROGRAM  CODE HERE AND SAVE 
            
            
    B)  DOWNLOAD A .wav SOUND CLIP TO BROADCAST , IN THE SAME FOLDER or DOWNLOAD IT FROM REPOSITRY...IN MY CASE IT IS star-wars.wav   
    
    C) COMPILE THAT C FILE USING FOLLOWINg COMMANDS:
                  $ gcc  -lm -std=c99 -g my_fm.c -o my_fm
                 
    D) RUN THE my_fm FILE WITH ARGUMENTS ->   .wav TYPE SOUND AND THE FREQUENCY @ WHICH U WANT TO  BROADCAST
            
                 $ ./my_fm ./star-wars.wav 100.0 
                 
                 
    
