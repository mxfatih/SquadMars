# SquadMars
A squad mission on planet Mars. Which you move them on an Rectangular area remotely.

Project developed in .Net Core 3.0 as Rest API.

You start with setting Target area borders.

For ex:

To Set Area as (0,0) to (5,5):

https://localhost:44357/squad/SetAreaEndPoint?area=5%205

Then add Rover to your Squad by sending a start Point (1,2) and Direction(Any cardinal Compass value[N, E, S, W]):

https://localhost:44357/squad/AddRover?rover=1%202%20N

Then send a Command text which each letter is 1 command[L, R, M])
L, R - > Rotate Rover 90 degree to the left or right
M -> Move Rover 1 unit

https://localhost:44357/squad/MoveRover?memberId=0&commandText=LMLMLMLMM
