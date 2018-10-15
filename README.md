```
                                                                                    
                                                                       ,''''.       
                                                                     :;      ',     
  @@@@@@`                  #@@@.                                    '    `    `'    
  @@@@@@,                 +@@@@@`                                  '     `      ;   
  @@,``..                 @@:..@@                                 .`     `      ,`  
  @@`      `      `      :@:`  ':   `                 ,           '      `       '  
  @@`     @@@;  '@@@     @@,       @@@,@ @#+@@.+@@:  @@@; ,@#     ,      `       ;  
  @@@@@@ @@'@@` @@'@@    @@.      @@''@@,@@@;@@@;@@ @@:#@`@#:    .       `       `  
  @@@@@@`@:` @++@, `@.   @@`   #@ @+. #@,@@, #@: #@`@:` @:@;     , ``````.````````` 
  @@,..,`@,  #@@#`  @,   @@`   +@,@:  `@,#@` +@. +@`@''@@'@@,    .       `       `  
  @@`   `@.  #@@#   @:   +@.   ;@,@,  `@.#@` +@` +@`@@@@#: @@`    .      `       :  
  @@`    @,  @##@   @,    @@   :@,@'  +@,#@` +@` +@`@:.`    @,    '      `       '  
  @@`    @@`+@:`@+ @@,    @@@,#@@,@@.,@@,#@` +@` +@`@@  @` ,@,    ,      `      .`  
  @@`    `@@@#. #@@@:      @@@@@@, @@@;@,#@` #@` #@` @@@@,@@@.     '     `      '   
   ,`     `';,   ,':`       ;+;,`` `+:.,, ,`  ,`  ,` `'':`.:,       '    `     '    
                                                                     ;:  `   ;;     
                                                                       :'''':       
                                                                                    
------------------------------------------------------------------------------
sm_foocrowbar | Foo's throwing Crowbars and Stun Sticks
Copyright (c) 2013 - 2018 Foo Games | www.foo-games.com <foobarhl@gmail.com>
Licensed under the GPLv3.  See LICENSE for terms.

Optional Support and Maintenance is available from www.foo-games.com

Donations also greatly appreciated!  Paypal: foobarhl@gmail.com
------------------------------------------------------------------------------


# [foo] bar's Throwing Crowbars and Stunsticks for Half-Life 2: Deathmatch.

## Installation

 1. Install addons/sourcemod/plugins/sm_foocrowbar.smx
 2. Load the plugin.  The plugin will auto create the configuration file if 
    not present (below)

## Upgrading from 0.18 or prior

Version 0.20 introduces changes to the cvars for sm_foocrowbar_explodedamage and 
sm_foocrowbar_exploderadius to make them more consistent with the env_explosion 
entity.

sm_foocrowbar_explodedamage now controls whether explosions are enabled and 
manages the magnitude of the explosion.  The new default for this cvar is 80.

sm_foocrowbar_exploderadius now overrides the radius of explosion.  
By default, the radius will be based on the magntitude set by 
sm_foocrowbar_explodedamage.

If you used 0.18, either update cfg/sourcemod/plugin.sm_foocrowbar.cfg or 
delete it to have the config rebuild.

 
## Configuration

Configuration: cfg/sourcemod/plugin.sm_foocrowbar.cfg

### General Settings

  sm_foocrowbar_explodedamage : Damage magnitude to inflict when a crowbar explodes (0 to disable explosions)
  sm_foocrowbar_exploderadius : Radius override of explosion (0 to scale against sm_foocrowbar_explodedamage)
  sm_foocrowbar_maxlife       : How long for crowbars to stay in the map   after being thrown
  sm_foocrowbar_maxperspawn   : How many thrown crowbars a player can have  per-spawn
  sm_foocrowbar_mintime       : Minimum time between throwing a crowbar
  sm_foocrowbar_throwndamage  : How much damage to inflict on a player when hit by a crowbar/stunstick
  sm_foocrowbar_debug         : Enable console debugging of the plugin

### Admin Flag Requirements ###
  sm_foocrowbar_requiredflag  : Specifies what admin flag is required to use the plugin.  Leave "" to not required

### Donator Support ###

  sm_foocrowbar_donator_level     : Minimum level required to use throwing crowbars/stunsticks.  
                                    Leave at 0 to not require donation access to throw crowbars

  sm_foocrowbar_maxperspawn_level : Number of throwing crowbars to give a donator.  
                                    If sm_foocrowbar_donator_level is 0, then 
                                    donators will get this amount of crowbars 
                                    but regular players will get 
                                    sm_foocrowbar_maxperspawn instead.

### Tips 'n tricks ###

Q: Throwing things requires no skill!  It's too spammy!
A: Fiddle with the settings.  Throwing knives has proven to be pretty fun in
   CSS.

## Change Log ##
 * 0.20 : Correct an issue with explosions not working due to prop_physics change in previous version.  NOTE:  CVARS HAVE CHANGED IN THIS VERSION
 * 0.18 : Fixed a problem with donator interface on servers without donator installed.
 * 0.17 : Added simple donator interface support.  New cvars:  sm_foocrowbar_donator_level  and sm_foocrowbar_donator_maxperspawn
 * 0.16 : Added admin flag requirement support.  New cvar is  sm_foocrowbar_requiredflag
 * 0.15 : Fixed an issue causing two bars to be thrown at once
 * 0.14 : Added stunsticks
 * 0.13 : First stable release.  Fixes an issue with trigger impacts at crowbars
 * 0.12 : Private beta test.


^D
```