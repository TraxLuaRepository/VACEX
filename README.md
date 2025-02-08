# VACEX
Vacex - A external prioritizing your safety while maintaining "Good" features.


# LUA DOCUMENTATION

- Classes
> Game_Class
```lua
local EntityList = game:GetEntityList()
local GameMode = game:GetGameMode() -- DeathMatch, Casual, Competitive, Premier
local PlantedC4 = game:GetC4() -- C4_Class
local CSGOInput = game:GetCSGOInput() -- CSGO_Input_Class
local LocalPlayer = game:GetLocalPlayer() -- Player_Class
local Input = game:GetInput() -- Input_Class
```
> Input_Class
```lua
local Input = game:GetInput()
local IsShooting = Input.IsShooting
local IsAiming = Input.IsAiming
local MoveDirection = Input.MoveDirection
local IsRight = Input.Right
local IsLeft = Input.Left
local Forward = Input.Forward
local Backwards = Input.Backwards

-- Functions
Input:Shoot(PARAMETERS: Delay (INT), Until (INT), MATCH (BOOL))
-- Explaination. Until will shoot until INT ms have passed. Delay delays it. Match means if the bool you attach to it is true, it shoots, if not it stops.
Input:Aim(PARAMETERS: Delay, Until(INT), Match (BOOL))
-- Explaination, same as before.
```
