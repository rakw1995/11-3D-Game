# Graveyard Smash
* This repository is Graveyard Smash, a 3d game I have made in Godot.

* Graveyard Smash is a vaporwave & 80s inspired miniature adventure in which you play as a young witch trapped in a graveyard at night. Your goal is to fight off the creatures who haunt the night with your magic.

- Assets:
  - Graveyard set: Kenney.nl
  - Creatures: Kenney.nl
  - Music: https://opengameart.org/content/the-crypt
  - Sound Effects: 
  - Menu screen: designed by me in Adobe Photoshop
  - Fonts: dafont.com
  - Icon & Menu Ghosts: made by me in Adobe Illustrator
  - Mouse: Kenney.nl, edited by me using Adobe Photoshop)
  
 * Creation Steps:
  - MENU SCREEN: 
  - GRAVEYARD SCENE:
  - GAME OVER SCREEN:
  - FIREBALL:
  - GHOSTS:
    - instanced ghosts as kinematic body so that they could move and interact with player
    - added script that uses detect_radius to follow the player when in range.
  - PLAYER/CONTROLS: 
    - project settings > input map > added left, right, forward, and back movement controls that i referenced in script witch.gd to control movement with keys
    - unhandled input function added to script to deal with mouse movement connecting to camera (pivot node & child)
    - physics process function added to ensure nothing weird happens with gravity and/or movement
    
  - EFFECTS/POST-PROCESSING:
    - fog: graveyard > add child node > world environment > fog enabled, depth enabled, > set depth end to 540 (leave begin at 0)
    - change sun color to red ( world environment > background > sun > sun color )
    - change lighting effects: world environment > tonemap > changed exposure to .8, changed mode to "aces"
  - AUDIO:
    - Music: Add child node > audio stream player > set to autoplay
    - SFX: Add child node > audio stream player > do not auto play > add script to define when playing = true
  
  

  

