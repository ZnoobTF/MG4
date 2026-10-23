# MG4
## Devlog
The FloatAnimation script on the start of the game (inside the Start method) sets the float variable _timer to a float variable _switchspeed. This can be customized, but by default
is set to 3.0. Every frame, the code runs in the Update() method, which moves the animation up or down based on a boolean variable _up. There is an if else statement that
does this, and the speed it goes up and down can be modified by the _movespeed variable, default is 5.0. The amount the object moves is based on how much time passed since the last frame,
Time.deltaTime, and the _movespeed variable. After the if else statement, our _timer variable is set to itself subtracted by the Time.deltaTime. Then, we check in an if statement
if our _timer variable is below or equal to 0. If it is, we reset the _timer variable to the +switchspeed variable, and the variable _up is set to the opposite of itself, so that for the next _switchSpeed or greater amount of time, depending on frames
the object will go in the opposite direction. 

## Open-Source Assets
- [Quirky animal 3D models](https://assetstore.unity.com/packages/3d/characters/animals/quirky-series-free-animals-pack-178235)
- [City 3D models](https://assetstore.unity.com/packages/3d/environments/simplepoly-city-low-poly-assets-58899)
- [Bite sound effect](https://freesound.org/people/Jofae/sounds/353067/)