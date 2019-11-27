# proppfrexx-remote
Example settings for Proppfrexx playout software with D&amp;R Airlite mixer

This project is inspired by and based upon the work of [Benjamin Hartwich](https://github.com/benhartwich/proppfrexx-remote).

I've made numerous changes to Ben's config which are explained in detail on my blog [radiotech.nl](https://www.radiotech.nl).

### proppfrexx-remote \ 2-players
Presets: 
- **2 DJ players in ProppFrexx** to play tracks from your main program playlist.
  - DJ player A is linked to Airlite channel 4.
  - DJ player B is linked to Airlite channel 5. 
- **2 Standby players** for ad-hoc content like interviews or additional audio clips.
  - Both standby players are linked to Airlite channel 7.
- **2 Cartwalls** for playing jingles, beds, fillers, closers etcetera. 
  - Cartwall 1 is linked to Airlite channel 6 and controlled by Controls A1 through A8.
  - Cartwall 2 is linked to Airlite channel 7 and controlled by Controls B1 through B8. 
- **1 PFL-player**, for Pre Fade Listening of content off-air. 
  - Pre Fade Listening for all Airlite channels is rerouted to Airlite channel 7.
  
Airlite configuration:
- **Airlite Configuration** file contains preferences for the Airlite modules 1 through 8 and Master:
  - airlite.config: Use Airlite Configuration Manager to load the recommended presets into your D&R Airlite mixer.

ProppFrexx configuration: 
- **ProppFrexx output/input channels** links ProppFrexx to Airlite mixer input/output streams:
  - proppfrexx.mixer: Store in %APPDATA%\Radio42\ProppFrexx ONAIR\4.0 then activate using ProppFrexx > Settings > Input/Output.
- **ProppFrexx routing** (define mixers channels for all ProppFrexx player types including DJ players, PFL-player and cartwalls):
  - Todo: ProppFrexx > Settings > Input/Output.
  - Todo: Could this be used for alternative routing when using non-stop/auto play mode?
- **ProppFrexx events** (define events like starting/stopping tracks or carts using Airlite faders and Control buttons):
  - proppfrexx.events: Import into ProppFrexx using Settings > Events/commands.
- **ProppFrexx GPIOClient** (map Airlite Events like state changes per channel/module/button to ProppFrexx control comands):
  - Default.drl: Store in %APPDATA%\Radio42\ProppFrexx GPIOClient\4.0 then activate using ProppFrexx GPIOClient.
- **ProppFrexx workspace**:
  - Todo: ProppFrexx Workspace/view.
