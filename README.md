**Installation**
------------------
1. Download ProdigySim's recording helper plugin [here](https://steamcommunity.com/linkfilter/?url=https://github.com/ProdigySim/recording_helpers/releases/download/v0.6/recording_helpers-0.6-l4d.zip).      
Extract both the .dll and .vdf files into your addons folder.         
Skip this step if you already use the plugin.    

2. Download the zip with vpk addon here.   
Extract the VPK file to the addons folder.    

3. Remove the -lv (low violence) launch command if being used.

*Note: Changing resolutions resets parts of the cfg and requires a restart.

**Benchmarking**
------------------
**Don't expect the huge gains you see below with inferior hardware.**  
All results based on a three run sum average.    
All results are from load with the survivor view vomited and a large horde attacking on DT Map1.  
All results are from a recorded demo file for consistency.  

Test Setup: i5 2500k @ 4ghz / gtx 970 ssc+ / 8gb 1866mhz cl8 / w10 x64   
Video Settings: Everything disabled / Effect Detail Medium / Multicore Enabled / Memory High / 1080p / fps_max 0    


> **L4D Without FPS Boost**  
 302 frames 1.360 seconds **221.97 fps ( 4.50 ms/f )** 24.489 fps variability

         

> **L4D With FPS Boost**  
>  302 frames 0.702 seconds **429.97 fps ( 2.32 ms/f )** 44.956 fps variability
>  
> - 93% increase in frames per second
> - 48% decrease in latency to display a fresh frame
> - ( 1 second = 1000 ms ( 1000 ms / 429.97 fps = 2.32 ms/f ) ) e.g.:
>  - 60 fps = 16.6 ms/f
>  - 120 fps  = 8.3 ms/f

> [Sample profile](https://drive.google.com/open?id=0B15LgQ1PwzQpTjFtbUZSTkVvSjA) of a full map play-through.

         

> **L4D With FPS Boost, Threadpool Reserve 1**  
  302 frames 0.680 seconds **444.30 fps ( 2.25 ms/f)** 44.045 fps variability
 
> Settings a threadpool reserve will cause the client to hang when exiting the game, so it's left out of the config. If you'd like to use this, you will need to have a dedicated exit key bind that sets the threadpool to 0 then exits the game.

**Optional Settings**
---------
If you want fading ragdolls instead of instantly disappearing ragdolls, put `g_ragdoll_fadespeed 1` in your autoexec.

If you want less blurry textures and clearer spray images, put `mat_picmip 1` in your autoexec.

You can refer to the [Hidden CVAR](http://steamcommunity.com/sharedfiles/filedetails/?id=564185677) guide on Steam for more optional settings you can add to your autoexec.

**Crashing**
---------
If you experience random crashing, put `exec fix` in your autoexec.
