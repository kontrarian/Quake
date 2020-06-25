# Platform Specific Files

* sys_win.c 
    - Operating system interface code. 
    - Public interface found in `sys.h`
    - Uses `Sys_` as the namespace
* cd_win.c - CD audio code. Public interface found in `cdaudio.h`
* in_win.c - Non keyboard input devices. Public interface found in `input.h`. Includes mouse
* net_win.c -
    * net_wins.c -
    * net_wipx.c -
* snd_win.c - 
* vid_win.c - 

# Todo

- remove IPX support (drivers, menu options, net_wipx.h and net_wipx.c)
- remove non-windows code (check for all _WIN32, X11, __linux__, NeXT, __sun__)
- remove CD audio?
- remove support for running as a dedicated server
- remove non-keyboard input handling?
- fix compiler warnings
- ensure uniform code style and naming conventions
- update to use stdint and stdbool?
- figure out where to see the console output

# Glossary

edict_t - Entity Dictionary

# General

* IPX/SPX was an alternative network protocol to IP/TCP. Had better performance on lan but didn't scale well and ultimately lost to TCP/IP due to the popularity of the internet

* Host_Init() and Host_Frame() are the main entry points

* The quit screen had some cute quit messages for non-win32, maybe replace the default exit screen with them later. They were in menu.c under /* QUIT MENU */ as char *quitMessage[].

# Namespaces

Cache_
Chase_
Con_
COM_
Cmd_
Cbuf_
Draw_
Host_
Hunk_
IN_
M_
Memory_ 
Mod_
NET_
PR_
R_
SCR_
SV_
V_
VID_
W_
Z_