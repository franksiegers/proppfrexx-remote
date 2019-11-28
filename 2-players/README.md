# proppfrexx-remote / 2-players

## ProppFrexx Presets

ProppFrexx will be configured with the following players and routing: 

- **2 DJ players** to play tracks from your main program playlist.
  - DJ player A is linked to Airlite channel 4.
  - DJ player B is linked to Airlite channel 5. 
- **2 Standby players** for ad-hoc content like interviews and additional audio clips.
  - Standby player 1 is linked to Airlite channel 7.
  - Standby player 2 is also linked to Airlite channel 7.
- **2 Cartwalls** for playing jingles, beds, fillers, closers etcetera. 
  - Cartwall 1 is linked to Airlite channel 6 and controlled by Airlite control buttons A1 through A8.
  - Cartwall 2 is linked to Airlite channel 7 and controlled by Airlite control buttons B1 through B8. 
- **1 PFL-player**, for Pre Fade Listening (off-air audio check). 
  - Pre Fade Listening for all Airlite channels is rerouted to Airlite channel 7.
  
## Airlite configuration

- **Airlite module preferences** Sets CRM mute and led switch colors for channels 1 through 8 and cue switches. 
  - Import airlite.prefs.xml into Airlite Configuration Manager to set preferences for all D&R Airlite modules. 
 
## ProppFrexx configuration

- **ProppFrexx Input/Output** - Links ProppFrexx mixer channels to Airlite USB input/output streams.
  - Store proppfrexx.mixer in %APPDATA%\Radio42\ProppFrexx ONAIR\4.0 then activate using ProppFrexx > Settings > Input/Output.
  
- **ProppFrexx Routing** - Defines Routing for all ProppFrexx players to specific ProppFrexx mixer channels.
  - Todo: ProppFrexx > Settings > Input/Output.
  - Todo: Could this be used for alternative routing when using non-stop/auto play mode?
  
- **ProppFrexx Events** - Defines ProppFrexx events like starting tracks/carts using Airlite faders and control switches.
  - Import proppfrexx.events into ProppFrexx using Settings > Events/commands.
  
- **ProppFrexx GPIOClient** - Maps Airlite Events like fader/switch state changes to ProppFrexx control comands.
  - Store Default.drl in %APPDATA%\Radio42\ProppFrexx GPIOClient\4.0 then activate using ProppFrexx GPIOClient.
  
- **ProppFrexx workspace** - Defines the layout and settings for the ProppFrexx Graphical User Interface (GUI).
  - Todo: ProppFrexx Workspace/view.

.