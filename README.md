# VACEX
Vacex - A external prioritizing your safety while maintaining "Good" features.


# Lua Documentation

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
local Input = game:GetInput() -- Input_Class
local IsShooting = Input.IsShooting -- bool
local IsAiming = Input.IsAiming -- bool
local MoveDirection = Input.MoveDirection -- Vector3
local IsRight = Input.Right -- bool
local IsLeft = Input.Left -- bool
local Forward = Input.Forward -- bool
local Backwards = Input.Backwards -- bool
local Entity_On_Mouse = Input.MouseHit -- Player_Class

-- Functions
Input:Shoot(PARAMETERS: Delay (INT), Until (INT), MATCH (BOOL))
-- Explaination. Until will shoot until INT ms have passed. Delay delays it. Match means if the bool you attach to it is true, it shoots, if not it stops.
Input:Aim(PARAMETERS: Delay, Until(INT), Match (BOOL))
-- Explaination, same as before.
```
> Player_Class
```lua
local Player = game:GetLocalPlayer()
local Health = Player.Health
local Armor = Player.Armor
local EquippedWeapon = Player.Weapon -- Weapon_Class
local Bones = Player:GetBones() -- Bone_Class
local InBuyZone = Player.IsInBuy
local AimPunchAngle = Player.AimPunchAngle -- QAngle
local AimPunchAngleVelocity = Player.AimPunchAngleVelocity -- QAngle
local AimPunchBase = Player.AimPunchBase -- Int
local IsInLanding = Player.IsInLanding -- bool
local IsBuyMenuOpen = Player.BuyMenuOpen -- bool
local Velocity = Player.Velocity -- Vector3
local Flags = Player.Flags -- Int
local EyeAngles = Player.EyeAngles -- Vector3
local Name = Player.Name -- String
local CameraServices = Player:GetCamera() -- Camera_Class
```
> Bone_Class
```lua
local Bones = Player:GetBones()
local Head = Bones.Head -- Part
local Torso = Bones.Torso -- Part
local RightShoulder = Bones.RightShoulder -- Part
local LeftShoulder = Bones.LeftShoulder -- Part
local Spine = Bones.Spine -- Part
local Spine_1 = Bones.Spine1 -- Part
local LeftArm = Bones.LeftArm -- Part
local RightArm = Bones.RightArm -- Part
local LeftHand = Bones.LeftHand -- Part
local RightHand = Bones.RightHand -- Part
left LeftHip = Bones.LeftHip -- Part
local RightHip = Bones.RightHip -- Part
local LeftKnee = Bones.LeftKnee -- Part
local RightKnee = Bones.RightKnee -- Part
local LeftFoot = Bones.LeftFoot -- Part
Local RightFoot = Bones.RightFoot -- Part
```
> Part
```lua
local Position = Part.Position -- vector3
local Name = Part.Name -- string
local Part_ID = Part.ID -- int
```
