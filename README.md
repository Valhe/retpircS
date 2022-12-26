--Envidioso DHAT



if game.PlaceId == 9824221333 then
  local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
  local Window = Library.CreateLib("DHAT - retpircS#8599", "Sentinel")
  local Main = Window:NewTab("Principal")
  local Tepe = Window:NewTab("Tp")
  local Otros = Window:NewTab("Otros")
  local Credits = Window:NewTab("retpircS#8599")
  
  
  
  
--locals
local Lp = game.Players.LocalPlayer


--Abrir Cerrar

  local OpenClose = Main:NewSection("Open/Close")
OpenClose:NewKeybind("Choose", "", Enum.KeyCode.Z, function()
	Library:ToggleUI()
end) 
--Tp
  local TP = Tepe:NewSection("Tp")
   TP:NewButton("Food1", "Tp LocalPlayer To Food", function()
    Lp.Character.HumanoidRootPart.CFrame = CFrame.new(-133.079697, 839.824036, -12.509532, -0.993873417, -3.15072413e-08, -0.110524274, -3.9447027e-08, 1, 6.96508309e-08, 0.110524274, 7.3583962e-08, -0.993873417)
end)
  TP:NewButton("Metro", "Tp LocalPlayer To Metro", function()
    Lp.Character.HumanoidRootPart.CFrame = CFrame.new(-314.077179, 801.408142, -271.691895, -0.999790013, 3.57832897e-09, 0.0204931479, 3.33201666e-09, 1, -1.20533983e-08, -0.0204931479, -1.19825829e-08, -0.999790013)
end)
  TP:NewButton("Armor", "Tp LocalPlayer To Armor", function()
    Lp.Character.HumanoidRootPart.CFrame = CFrame.new(-916.155273, 835.459778, 330.390533, -1, 0, 0, 0, 1, 0, 0, 0, -1)
end)
  TP:NewButton("Food2", "Tp LocalPlayer To Food2", function()
    Lp.Character.HumanoidRootPart.CFrame = CFrame.new(-142.67334, 839.907043, -237.816452, -0.993079066, -3.13687529e-08, -0.117447577, -2.51884433e-08, 1, -5.41061453e-08, 0.117447577, -5.07733589e-08, -0.993079066)
end)
TP:NewButton("Casino", "Tp LocalPlayer To Casino", function()
    Lp.Character.HumanoidRootPart.CFrame = CFrame.new(-738.398254, 838.664673, 252.179581, 0.998647153, 1.12314034e-08, -0.0519981645, -6.81856926e-09, 1, 8.50425863e-08, 0.0519981645, -8.45729815e-08, 0.998647153)
end)




--Main




  local Exploits = Main:NewSection("Funciones")

Exploits:NewButton("NoClip(E)", "By Me", function()
    local noclip = false
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local mouse = player:GetMouse()

mouse.KeyDown:Connect(function(key)
    if key == "e" then
        noclip = not noclip

        if not StealthMode then
        end
    end
end)

while true do
    player = game.Players.LocalPlayer
    character = player.Character

    if noclip then
        for _, v in pairs(character:GetDescendants()) do
            pcall(function()
                if v:IsA("BasePart") then
                    v.CanCollide = false
                end
            end)
        end
    end

    game:GetService("RunService").Stepped:wait()
end
end)


 Exploits:NewButton("UIGOTO(BETA)", "BETA FOR ME", function()
      local CoreGui = game:GetService("StarterGui")

CoreGui:SetCore("SendNotification", {
    Title = "retpircS#8599",
    Text = "retpircS#8599",
    Duration = 2.5,
})

local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local TextBox = Instance.new("TextBox")
local TextButton = Instance.new("TextButton")

ScreenGui.Parent = game.CoreGui

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.new(8,0,0)
Frame.BorderColor3 = Color3.new(0.67451, 0.211765, 0.152941)
Frame.Position = UDim2.new(0.9,0.5,0.3)
Frame.Size = UDim2.new(0.07,0.1,0.1)
Frame.Active = true
Frame.Draggable = false

TextBox.Parent = Frame
TextBox.BackgroundColor3 = Color3.new(5,5,5)
TextBox.BackgroundTransparency = 0
TextBox.Position = UDim2.new(0.103524067, 0, 0.200333327, 0)
TextBox.Size = UDim2.new(0.8,0.9,0.6)
TextBox.Font = Enum.Font.SourceSansLight
TextBox.FontSize = Enum.FontSize.Size14
TextBox.Text = "Name"
TextBox.TextScaled = true
TextBox.TextSize = 8
TextBox.TextWrapped = true

TextButton.MouseButton1Click:connect(function()
end)

local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local TextButton = Instance.new("TextButton")


ScreenGui.Parent = game.CoreGui

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.new(8,0,0)
Frame.BorderColor3 = Color3.new(0.67451, 0.211765, 0.152941)
Frame.Position = UDim2.new(0.9,0.5,0.4)
Frame.Size = UDim2.new(0.07,0.1,0.1)
Frame.Active = true
Frame.Draggable = false

TextButton.Parent = Frame
TextButton.BackgroundColor3 = Color3.new(5,5,5)
TextButton.BackgroundTransparency = 0
TextButton.Position = UDim2.new(0.103524067, 0, 0.200333327, 0)
TextButton.Size = UDim2.new(0.8,0.9,0.6)
TextButton.Font = Enum.Font.SourceSansLight
TextButton.FontSize = Enum.FontSize.Size14
TextButton.Text = "Teleport"
TextButton.TextScaled = true
TextButton.TextSize = 8
TextButton.TextWrapped = true

TextButton.MouseButton1Click:connect(function()
local lplayer = game:GetService('Players').LocalPlayer
 
local yeeting = false
function GetPlayer(String)
local Found = {}
local strl = String:lower()
if strl == "all" then
for i,v in pairs(game:GetService("Players"):GetPlayers()) do
table.insert(Found,v)
end
elseif strl == "Random" then
for i,v in pairs(game:GetService("Players"):GetPlayers()) do
if v.Name ~= lplayer.Name then
table.insert(Found,v)
end
end 
elseif strl == "me" then
for i,v in pairs(game:GetService("Players"):GetPlayers()) do
if v.Name == lplayer.Name then
table.insert(Found,v)
end
end 
else
for i,v in pairs(game:GetService("Players"):GetPlayers()) do
if v.Name:lower():sub(1, #String) == String:lower() then
table.insert(Found,v)
end
end 
end
return Found 
end
function ahh(thing)
local asd = {'yeet','gui','yeet gui'}
local f = string.upper(asd[math.random(1,#asd)])
return f
end

local target = unpack(GetPlayer(TextBox.Text)).Character
 
game:GetService'Players'.LocalPlayer.Character.HumanoidRootPart.CFrame = target.Head.CFrame;coin.Location = target.Head.Position game["Run Service"].Heartbeat:wait()
end)
end)

  
  
  Exploits:NewButton("Antilock", "Antilock", function()
      getgenv().antilock = true 
 
game:GetService("RunService").heartbeat:Connect(function()
    if getgenv().antilock == true then 
    local abc = game.Players.LocalPlayer.Character.HumanoidRootPart.Velocity
    game.Players.LocalPlayer.Character.HumanoidRootPart.Velocity = Vector3.new(1,1,1) * (2^16)
    game:GetService("RunService").RenderStepped:Wait()
    game.Players.LocalPlayer.Character.HumanoidRootPart.Velocity = abc
    end 
end)
end)
  
  Exploits:NewButton("Fly Alt", "Toca Alt para Volar", function()
      local Settings = {
	
	Speed = 5,
	SprintSpeed = 30,
	ToggleKey = Enum.KeyCode.LeftAlt,
	SprintKey = Enum.KeyCode.LeftControl,
	
	ForwardKey = Enum.KeyCode.W,
	LeftKey = Enum.KeyCode.A,
	BackwardKey = Enum.KeyCode.S,
	RightKey = Enum.KeyCode.D,
	UpKey = Enum.KeyCode.E,
	DownKey = Enum.KeyCode.Q,
	
}

local Screen = Instance.new("ScreenGui",game.CoreGui)
local Distance = Instance.new("TextLabel",Screen)
Distance.BackgroundTransparency = 1
Distance.Size = UDim2.new(0,10,0,10)
Distance.ZIndex = 2
Distance.Text = "0"
Distance.TextStrokeTransparency = .5
Distance.TextSize = 20
Distance.TextStrokeColor3 = Color3.fromRGB(33, 33, 33)
Distance.Font = Enum.Font.Gotham
Distance.TextColor3 = Color3.new(1,1,1)
Distance.TextXAlignment = Enum.TextXAlignment.Left
Distance.TextYAlignment = Enum.TextYAlignment.Top


local Mouse = game.Players.LocalPlayer:GetMouse()
local Direction = Vector3.new(0,0,0)
local InterpolatedDir = Direction
local Tilt = 0
local InterpolatedTilt = Tilt
local RunService = game:GetService("RunService")
local Toggled = false
local Sprinting = false
local CameraPos = game.Workspace.CurrentCamera.CFrame.Position

pcall(function()
	game.Players.LocalPlayer.DevCameraOcclusionMode = Enum.DevCameraOcclusionMode.Invisicam	
end)

function Lerp(a, b, t)
    return a + (b - a) * t
end

local LastPos = nil

function KeyHandler(actionName, userInputState)
	if true and game.Players.LocalPlayer.Character and game.Players.LocalPlayer.Character:FindFirstChild("HumanoidRootPart") then
		if actionName == "Toggle" and userInputState == Enum.UserInputState.Begin then
			Toggled = not Toggled
			if Toggled then
				LastPos = game.Players.LocalPlayer.Character.HumanoidRootPart.Position
				--game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = true
				game.Players.LocalPlayer.Character.Humanoid.PlatformStand = true 
			else
				LastPos = nil
				game.Players.LocalPlayer.Character.Humanoid.PlatformStand = false
				--game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = false
			end
		elseif actionName == "Forward" then
			Tilt = userInputState == Enum.UserInputState.Begin and -20 or 0
			Direction = Vector3.new(Direction.x,Direction.y,userInputState == Enum.UserInputState.Begin and -1 or 0)
		elseif actionName == "Left" then
			Direction = Vector3.new(userInputState == Enum.UserInputState.Begin and -1 or 0,Direction.y,Direction.z)
		elseif actionName == "Backward" then
			Tilt = userInputState == Enum.UserInputState.Begin and 20 or 0
			Direction = Vector3.new(Direction.x,Direction.y,userInputState == Enum.UserInputState.Begin and 1 or 0)
		elseif actionName == "Right" then
			Direction = Vector3.new(userInputState == Enum.UserInputState.Begin and 1 or 0,Direction.y,Direction.z)
		elseif actionName == "Up" then
			Direction = Vector3.new(Direction.x,userInputState == Enum.UserInputState.Begin and 1 or 0,Direction.z)
		elseif actionName == "Down" then
			Direction = Vector3.new(Direction.x,userInputState == Enum.UserInputState.Begin and -1 or 0,Direction.z)
		elseif actionName == "Sprint" then
			Sprinting = userInputState == Enum.UserInputState.Begin
		end
	end
end



game:GetService("UserInputService").InputBegan:connect(function(inputObject, gameProcessedEvent)
	
	if inputObject.KeyCode == Settings.ToggleKey then
		KeyHandler("Toggle", Enum.UserInputState.Begin, inputObject)
	elseif inputObject.KeyCode == Settings.ForwardKey then
		KeyHandler("Forward", Enum.UserInputState.Begin, inputObject)
	elseif inputObject.KeyCode == Settings.LeftKey then
		KeyHandler("Left", Enum.UserInputState.Begin, inputObject)
	elseif inputObject.KeyCode == Settings.BackwardKey then
		KeyHandler("Backward", Enum.UserInputState.Begin, inputObject)
	elseif inputObject.KeyCode == Settings.RightKey then
		KeyHandler("Right", Enum.UserInputState.Begin, inputObject)
	elseif inputObject.KeyCode == Settings.UpKey then	
		KeyHandler("Up", Enum.UserInputState.Begin, inputObject)
	elseif inputObject.KeyCode == Settings.DownKey then
		KeyHandler("Down", Enum.UserInputState.Begin, inputObject)
	elseif inputObject.KeyCode == Settings.SprintKey then
		KeyHandler("Sprint", Enum.UserInputState.Begin, inputObject)
	end
	
	
end)


game:GetService("UserInputService").InputEnded:connect(function(inputObject, gameProcessedEvent)
	
	if inputObject.KeyCode == Settings.ToggleKey then
		KeyHandler("Toggle", Enum.UserInputState.End, inputObject)
	elseif inputObject.KeyCode == Settings.ForwardKey then
		KeyHandler("Forward", Enum.UserInputState.End, inputObject)
	elseif inputObject.KeyCode == Settings.LeftKey then
		KeyHandler("Left", Enum.UserInputState.End, inputObject)
	elseif inputObject.KeyCode == Settings.BackwardKey then
		KeyHandler("Backward", Enum.UserInputState.End, inputObject)
	elseif inputObject.KeyCode == Settings.RightKey then
		KeyHandler("Right", Enum.UserInputState.End, inputObject)
	elseif inputObject.KeyCode == Settings.UpKey then	
		KeyHandler("Up", Enum.UserInputState.End, inputObject)
	elseif inputObject.KeyCode == Settings.DownKey then
		KeyHandler("Down", Enum.UserInputState.End, inputObject)
	elseif inputObject.KeyCode == Settings.SprintKey then
		KeyHandler("Sprint", Enum.UserInputState.End, inputObject)
	end
	
	
end)


RunService.RenderStepped:Connect(function()
	if Toggled and game.Players.LocalPlayer.Character and game.Players.LocalPlayer.Character:FindFirstChild("HumanoidRootPart")  then
		for i,v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
			if v:IsA("BasePart") then
				v.Velocity = Vector3.new(0,0,0)
			end
		end
		local RootPart = game.Players.LocalPlayer.Character.HumanoidRootPart
		if LastPos then
			Distance.Text = math.floor((LastPos-RootPart.Position).Magnitude+.5)
			if (LastPos-RootPart.Position).Magnitude >= 350 then
				Distance.TextColor3 = Color3.new(1,0,0)
			else
				Distance.TextColor3 = Color3.new(1,1,1)	
			end
		else
			Distance.TextColor3 = Color3.new(1,1,1)
			Distance.Text = 0
		end
		InterpolatedDir = InterpolatedDir:Lerp((Direction * (Sprinting and Settings.SprintSpeed or Settings.Speed)),.2)
		InterpolatedTilt = Lerp(InterpolatedTilt ,Tilt* (Sprinting and 2 or 1),Tilt == 0 and .2 or .1)
		RootPart.CFrame = RootPart.CFrame:Lerp(CFrame.new(RootPart.Position,RootPart.Position + Mouse.UnitRay.Direction) * CFrame.Angles(0,math.rad(00),0) * CFrame.new(InterpolatedDir)  * CFrame.Angles(math.rad(InterpolatedTilt),0,0),.2)
	else
		Distance.TextColor3 = Color3.new(1,1,1)
		Distance.Text = 0
	end	
end)
 
end)


  Exploits:NewButton("Silent C", "By kal", function()
      
-- script bought by kal (private request)


--[[

KKKKKKKKK    KKKKKKK               AAA               LLLLLLLLLLL             
K:::::::K    K:::::K              A:::A              L:::::::::L             
K:::::::K    K:::::K             A:::::A             L:::::::::L             
K:::::::K   K::::::K            A:::::::A            LL:::::::LL             
KK::::::K  K:::::KKK           A:::::::::A             L:::::L               
  K:::::K K:::::K             A:::::A:::::A            L:::::L               
  K::::::K:::::K             A:::::A A:::::A          22 L:::::L               
  K:::::::::::K             A:::::A   A:::::A          L:::::L               
  K:::::::::::K            A:::::A     A:::::A         L:::::L               
  K::::::K:::::K          A:::::AAAAAAAAA:::::A        L:::::L               
  K:::::K K:::::K        A:::::::::::::::::::::A       L:::::L               
KK::::::K  K:::::KKK    A:::::AAAAAAAAAAAAA:::::A      L:::::L         LLLLLL
K:::::::K   K::::::K   A:::::A             A:::::A   LL:::::::LLLLLLLLL:::::L
K:::::::K    K:::::K  A:::::A               A:::::A  L::::::::::::::::::::::L
K:::::::K    K:::::K A:::::A                 A:::::A L::::::::::::::::::::::L
KKKKKKKKK    KKKKKKKAAAAAAA                   AAAAAAALLLLLLLLLLLLLLLLLLLLLLLL


]]


--[[


                       _            _                _             _   
                      ( )          ( )              ( )           (_ ) 
  ___ ___     _ _    _| |   __     | |_    _   _    | |/')    _ _  | | 
/' _ ` _ `\ /'_` ) /'_` | /'__`\   | '_`\ ( ) ( )   | , <   /'_` ) | | 
| ( ) ( ) |( (_| |( (_| |(  ___/   | |_) )| (_) |   | |\`\ ( (_| | | | 
(_) (_) (_)`\__,_)`\__,_)`\____)   (_,__/'`\__, |   (_) (_)`\__,_)(___)
                                          ( )_| |                      
                                          `\___/'                      
-- Moongod Modfified (Switched out metatables / airshot and Sorted things out optimzing it)
-- Was this fully made by kal? fuck no bro its literally skidded but skidded inna good way no1 
seen before so yes its good


]]

    --[[ set Values to
        true if you want it to show
        false if not
    --]]
    
    -- Configurations
    --[[
    CLose = HumanoidRootPart / 0.120689803 Predict /  0.132 Accomdation / No AIRSHOT
    Mid = HumanoidRootPart / 0.141 Predict / 0.135 Accomdation / No AIRSHOT
    Far = 121 Predict / 0.138 Accomdation / Airshot true
    
                ^ My Sets


       // -- = -- sets  -- = -- \\
      |       astro  - 0.109     |
      |       astro  - 0.115     |
      |       astro  - 0.121     |
      |       astro  - 0.135     |
      |       astro  - 0.132     |
      |       silent - 0.1325    |     
      |       silent - 0.119     |     
      |       silent - 0.112     |
      // -- = -- holy  -- = -- \\
    ]]
    

--[[
        _G.Types = {
            Ball = Enum.PartType.Ball,
            Block = Enum.PartType.Block, 
            Cylinder = Enum.PartType.Cylinder
        }
        
        --variables                 
            local Tracer = Instance.new("Part", game.Workspace)
        Tracer.Name = "gay"
        Tracer.Shape = _G.Types.Ball
        Tracer.Material = "ForceField"
        Tracer.Size = Vector3.new(7,7,7)
        game:GetService("RunService").RenderStepped:Connect(function()
        Tracer.Transparency = Options.MySlider.Value
        Tracer.Color = Options.ColorPicker.Value
        end)
        --]]
    Settings = {
        Kalslock = {
        Enabled = true,
        Key = "c",
        showdot = true,
        airshots = false,
        notifaction = false,
        pingprediction = false,
        FOV = math.huge,
        RESOVLER = false,
        Tracer = false,
        TracerColor = Color3.new(0, 255, 238),
        TracerTransparency = 0.75,
        TracerThickness = 5,
        Circles = false,
        CircleFOV = 500,
        CircleColor = Color3.new(255, 255, 255),
        CircleThickness = 2,
        CircleFilled = false,
        CircleTransparency = 0.10,
        CircleTransparencyOutline = 0,
        OutlineColor = Color3.new(255, 255, 255),
        Texts = false, 
        TextColor = Color3.new(255, 255, 255),
        TextSize = 35,
        TextInput = "made by kal",
        Hitbox = true,
        NoBulletDelay = true,
        Autoclicker = true,
        AutoclickerTime = 0.01,
        AutoclickerKey = "v",
        AnimationPack = false
    
}
}

--[[
    Parts - / HumanoidRootPart / LowerTorso / UpperTorso / Head 
]]

        local SelectedPart = "HumanoidRootPart"
        local Prediction = true
        local PredictionValue = 0.1429
        


 local AnchorCount = 0
            local MaxAnchor = 50

                local CC = game:GetService"Workspace".CurrentCamera
                    local Plr;
                        local enabled = false
                            local accomidationfactor = 0.132
                local mouse = game.Players.LocalPlayer:GetMouse()
                    
                            local Inset = game:GetService("GuiService"):GetGuiInset().Y
                local Line = Drawing.new("Line")
                    local Text = Drawing.new("Text")
                          local Circle = Drawing.new("Circle")
                          local Circle1 = Drawing.new("Circle")
                          
                          
                           _G.Types = {
            Ball = Enum.PartType.Ball,
            Block = Enum.PartType.Block, 
            Cylinder = Enum.PartType.Cylinder
        }
                          
                          local placemarker = Instance.new("Part", game.Workspace)
                          placemarker.Shape = _G.Types.Ball
                          placemarker.Material = "ForceField"
                          placemarker.Color = Color3.new(0, 1, 1)

    function makemarker(Parent, Adornee, Color, Size, Size2)
        local e = Instance.new("BillboardGui", Parent)
        e.Name = "PP"
        e.Adornee = Adornee
        e.Size = UDim2.new(Size, Size2, Size, Size2)
        e.AlwaysOnTop = Settings.Kalslock.showdot
        local a = Instance.new("Frame", e)
        if Settings.Kalslock.showdot == true then
        a.Size = UDim2.new(1, 0, 1, 0)
        else
        a.Size = UDim2.new(0, 0, 0, 0)
        end
        if Settings.Kalslock.showdot == true then
        a.Transparency = 0
        a.BackgroundTransparency = 0
        else
        a.Transparency = 1
        a.BackgroundTransparency = 1
        end
        a.BackgroundColor3 = Color
        local g = Instance.new("UICorner", a)
        if Settings.Kalslock.showdot == false then
        g.CornerRadius = UDim.new(0, 0)
        else
        g.CornerRadius = UDim.new(1, 1) 
        end
        return(e)
    end

    
    local data = game.Players:GetPlayers()
    function noob(player)
        local character
        repeat wait() until player.Character
        local handler = makemarker(guimain, player.Character:WaitForChild(SelectedPart), Color3.fromRGB(0, 255, 229), 0.3, 3)
        handler.Name = player.Name
        player.CharacterAdded:connect(function(Char) handler.Adornee = Char:WaitForChild(SelectedPart) end)


        spawn(function()
            while wait() do
                if player.Character then
                end
            end
        end)
    end

    for i = 1, #data do
        if data[i] ~= game.Players.LocalPlayer then
            noob(data[i])
        end
    end

    game.Players.PlayerAdded:connect(function(Player)
        noob(Player)
    end)

    spawn(function()
        placemarker.Anchored = true
        placemarker.CanCollide = false
        if Settings.Kalslock.showdot == true then
        placemarker.Size = Vector3.new(11, 11, 11)
        else
        placemarker.Size = Vector3.new(0, 0, 0)
        end
        if Settings.Kalslock.Hitbox == true then
        placemarker.Transparency = 0.30
        else
        placemarker.Transparency = 1
        end
        if Settings.Kalslock.showdot then
        makemarker(placemarker, placemarker, Color3.fromRGB(0, 255, 238), 0.80, 0)
        end
    end)

    game.Players.LocalPlayer:GetMouse().KeyDown:Connect(function(k)
        if k == Settings.Kalslock.Key and Settings.Kalslock.Enabled then
            if enabled == true then
                enabled = false
                if Settings.Kalslock.notifaction == true then
                    Plr = getClosestPlayerToCursor()
                game.StarterGui:SetCore("SendNotification", {
                    Title = "  Kal >3";
                    Text = "  Unlocked",
                    Icon = "http://www.roblox.com/asset/?id=5314810647",
                    Duration = 3
                })
            end
            else
                Plr = getClosestPlayerToCursor()
                enabled = true
                if Settings.Kalslock.notifaction == true then

                    game.StarterGui:SetCore("SendNotification", {
                        Title = "  Kal >3";
                        Text = "  Target: "..tostring(Plr.Character.Humanoid.DisplayName),
                        Icon = "http://www.roblox.com/asset/?id=8709610734",
                        Duration = 3
                    })

                end
            end
        end
    end)



    function getClosestPlayerToCursor()
        local closestPlayer
        local shortestDistance = Settings.Kalslock.FOV

        for i, v in pairs(game.Players:GetPlayers()) do
            if v ~= game.Players.LocalPlayer and v.Character and v.Character:FindFirstChild("Humanoid") and v.Character.Humanoid.Health ~= 0 and v.Character:FindFirstChild("HumanoidRootPart") then
                local pos = CC:WorldToViewportPoint(v.Character.PrimaryPart.Position)
                local magnitude = (Vector2.new(pos.X, pos.Y) - Vector2.new(mouse.X, mouse.Y)).magnitude
                if magnitude < shortestDistance then
                    closestPlayer = v
                    shortestDistance = magnitude
                end
            end
        end
        return closestPlayer
    end

    local pingvalue = nil;
    local split = nil;
    local ping = nil;

    game:GetService"RunService".Stepped:connect(function()
        if enabled and Plr.Character ~= nil and Plr.Character:FindFirstChild("HumanoidRootPart") then
            placemarker.CFrame = CFrame.new(Plr.Character.HumanoidRootPart.Position)
                            local Vector1 = CC:WorldToViewportPoint(Plr.Character.HumanoidRootPart.Position)
            Line.Color = Settings.Kalslock.TracerColor
                Line.Transparency = Settings.Kalslock.TracerTransparency
                Line.Thickness = Settings.Kalslock.TracerThickness
                Line.From = Vector2.new(mouse.X, mouse.Y + Inset)
                Line.To = Vector2.new(Vector1.X, Vector1.Y)
                Line.Visible = Settings.Kalslock.Tracer
                Text.Position = Vector2.new(mouse.X, mouse.Y + Inset)
                Text.Visible = Settings.Kalslock.Texts
                Text.Center = true
                Text.Outline = true
                Text.Font = 1
                Text.Size = Settings.Kalslock.TextSize
                Text.Color = Settings.Kalslock.TextColor
                Text.Text = Settings.Kalslock.TextInput
                Circle.Position = Vector2.new(mouse.X, mouse.Y + Inset)
                Circle.Visible = Settings.Kalslock.Circles
                Circle.Thickness = 1.5
                Circle.Thickness = Settings.Kalslock.CircleThickness
                Circle.Radius = Settings.Kalslock.CircleFOV
                Circle.Color = Settings.Kalslock.CircleColor
                Circle.Filled = Settings.Kalslock.CircleFilled
                Circle.Transparency = Settings.Kalslock.CircleTransparency
                Circle1.Visible = true
                Circle1.Radius = Settings.Kalslock.CircleTransparencyOutline
                Circle1.Position = Vector2.new(mouse.X, mouse.Y + Inset)
                Circle1.Thickness = 5
                Circle1.Color = Settings.Kalslock.OutlineColor

        else
                Circle.Visible = false
                Line.Visible = false
                Text.Visible = false
                Circle1.Visible = false
            placemarker.CFrame = CFrame.new(0, 9999, 0)
        end
        if Settings.Kalslock.pingprediction == true then
             pingvalue = game:GetService("Stats").Network.ServerStatsItem["Data Ping"]:GetValueString()
             split = string.split(pingvalue,'(')
             ping = tonumber(split[1])
            if ping < 130 then
                PredictionValue = 0.151
            elseif ping < 125 then
                PredictionValue = 0.149
            elseif ping < 110 then
                PredictionValue = 0.146
            elseif ping < 105 then
                PredictionValue = 0.138
            elseif ping < 90 then
                PredictionValue = 0.136
            elseif ping < 80 then
                PredictionValue = 0.134
            elseif ping < 70 then
                PredictionValue = 0.131
            elseif ping < 60 then
                PredictionValue = 0.1229
            elseif ping < 50 then
                PredictionValue = 0.1225
            elseif ping < 40 then
                PredictionValue = 0.1256
            end
        end
    end)

    local mt = getrawmetatable(game)
    local old = mt.__namecall
    setreadonly(mt, false)
    mt.__namecall = newcclosure(function(...)
        local args = {...}
        if enabled and getnamecallmethod() == "FireServer" and args[2] == "UpdateMousePos" and Settings.Kalslock.Enabled and Plr.Character ~= nil then

            -- args[3] = Plr.Character.HumanoidRootPart.Position+(Plr.Character.HumanoidRootPart.Velocity*accomidationfactor)
            --[[
            if Settings.Kalslock.airshots == true then
                if game.Workspace.Players[Plr.Name].Humanoid:GetState() == Enum.HumanoidStateType.Freefall then -- Plr.Character:WaitForChild("Humanoid"):GetState() == Enum.HumanoidStateType.Freefall
                    
                    --// Airshot
                    args[3] = Plr.Character.LeftFoot.Position+(Plr.Character.LeftFoot.Velocity*PredictionValue)

                else
                    args[3] = Plr.Character.HumanoidRootPart.Position+(Plr.Character.HumanoidRootPart.Velocity*PredictionValue)

                end
            else
    args[3] = Plr.Character.HumanoidRootPart.Position+(Plr.Character.HumanoidRootPart.Velocity*PredictionValue)
    end
    ]]
    if Prediction == true then
                
    args[3] = Plr.Character[SelectedPart].Position+(Plr.Character[SelectedPart].Velocity*PredictionValue)

    else

    args[3] = Plr.Character[SelectedPart].Position

    end

    return old(unpack(args))
    end
    return old(...)
    end)

    game:GetService("RunService").RenderStepped:Connect(function()
        if Settings.Kalslock.RESOVLER == true and Plr.Character ~= nil and enabled and Settings.Kalslock.Enabled then
        if Settings.Kalslock.airshots == true and enabled and Plr.Character ~= nil then
            
        if game.Workspace.Players[Plr.Name].Humanoid:GetState() == Enum.HumanoidStateType.Freefall then -- Plr.Character:WaitForChild("Humanoid"):GetState() == Enum.HumanoidStateType.Freefall
                


        if Plr.Character ~= nil and Plr.Character.HumanoidRootPart.Anchored == true then
        AnchorCount = AnchorCount + 1
        if AnchorCount >= MaxAnchor then
        Prediction = false
        wait(2)
        AnchorCount = 0;
        end
        else
        Prediction = true
        AnchorCount = 0;
        end

        SelectedPart = "LeftFoot"

        else
                

        if Plr.Character ~= nil and Plr.Character.HumanoidRootPart.Anchored == true then
        AnchorCount = AnchorCount + 1
        if AnchorCount >= MaxAnchor then
        Prediction = false
        wait(2)
        AnchorCount = 0;
        end
        
        else
        Prediction = true
        AnchorCount = 0;
        end

        SelectedPart = "HumanoidRootPart"

        end
        else

                

        if Plr.Character ~= nil and Plr.Character.HumanoidRootPart.Anchored == true then
        AnchorCount = AnchorCount + 1
        if AnchorCount >= MaxAnchor then
        Prediction = false
        wait(2)
        AnchorCount = 0;
        end
        else
         Prediction = true
         AnchorCount = 0;
        end
        SelectedPart = "HumanoidRootPart"
        end
        else
        SelectedPart = "HumanoidRootPart"
        end
        end)

        if Settings.Kalslock.NoBulletDelay == true then
            local FuckDelay = game:GetService("CorePackages").Packages
            FuckDelay:Destroy()
        end

        if Settings.Kalslock.Autoclicker == true then
            local time = Settings.Kalslock.AutoclickerTime --decrease if too slow increase if too fast
    
            click = false
            m = game.Players.LocalPlayer:GetMouse()
            m.KeyDown:connect(function(key)
            if key == Settings.Kalslock.AutoclickerKey then
            if click == true then click = false
            elseif
            click == false then click = true
            
            while click == true do 
            wait(time)
            mouse1click()
            end
            end
            end
            end)
        end
        
        if Settings.Kalslock.AnimationPack == true then
            -- Animation Pack --














for _, v in next, game:GetService("CoreGui"):GetChildren() do
    if (v.Name:match("Animation")) then
        v:Destroy()
    end
end

local Folder = Instance.new('Folder', game:GetService("Workspace"))
Folder.Name = ("Animation")

local LeanAnimation = Instance.new("Animation", Folder)
LeanAnimation.Name = "LeanAnimation"
LeanAnimation.AnimationId = "rbxassetid://3152375249"

local LayAnimation = Instance.new("Animation", Folder)
LayAnimation.Name = "LayAnimation"
LayAnimation.AnimationId = "rbxassetid://3152378852"

local Dance1Animation = Instance.new("Animation", Folder)
Dance1Animation.Name = "Dance1Animation"
Dance1Animation.AnimationId = "rbxassetid://3189773368"

local Dance2Animation = Instance.new("Animation", Folder)
Dance2Animation.Name = "Dance2Animation"
Dance2Animation.AnimationId = "rbxassetid://3189776546"

local GreetAnimation = Instance.new("Animation", Folder)
GreetAnimation.Name = "GreetAnimation"
GreetAnimation.AnimationId = "rbxassetid://3189777795"

local ChestPumpAnimation = Instance.new("Animation", Folder)
ChestPumpAnimation.Name = "ChestPumpAnimation"
ChestPumpAnimation.AnimationId = "rbxassetid://3189779152"

local PrayingAnimation = Instance.new("Animation", Folder)
PrayingAnimation.Name = "PrayingAnimation"
PrayingAnimation.AnimationId = "rbxassetid://3487719500"

if game.PlaceId == 2788229376 then
    function AnimationPack(Character)
        Character:WaitForChild'HumanoidRootPart'
        local Animation = Instance.new("ScreenGui")
        local AnimationPack = Instance.new("TextButton")
        local CloseButton = Instance.new("TextButton")
        local ScrollingFrame = Instance.new("ScrollingFrame")
        local ChestPumpButton = Instance.new("TextButton")
        local Dance1Button = Instance.new("TextButton")
        local Dance2Button = Instance.new("TextButton")
        local LayButton = Instance.new("TextButton")
        local GreetButton = Instance.new("TextButton")
        local LeanButton = Instance.new("TextButton")
        local PrayingButton = Instance.new("TextButton")

        Animation.Name = "Animation"
        Animation.Parent = game.CoreGui
        Animation.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

        AnimationPack.Name = "AnimationPack"
        AnimationPack.Parent = Animation
        AnimationPack.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        AnimationPack.BorderSizePixel = 0
        AnimationPack.Position = UDim2.new(0, 0, 0.5, 0)
        AnimationPack.Size = UDim2.new(0, 100, 0, 20)
        AnimationPack.Visible = false
        AnimationPack.Font = Enum.Font.SourceSansBold
        AnimationPack.Text = "Animations"
        AnimationPack.TextColor3 = Color3.fromRGB(0, 0, 0)
        AnimationPack.TextSize = 18.000

        CloseButton.Name = "CloseButton"
        CloseButton.Parent = AnimationPack
        CloseButton.BackgroundColor3 = Color3.fromRGB(255, 112, 112)
        CloseButton.Position = UDim2.new(0, 0, 0, 97)
        CloseButton.Size = UDim2.new(0, 120, 0, 25)
        CloseButton.Visible = false
        CloseButton.Font = Enum.Font.SourceSansBold
        CloseButton.Text = "CLOSE"
        CloseButton.TextColor3 = Color3.fromRGB(0, 0, 0)
        CloseButton.TextSize = 30.000

        ScrollingFrame.Parent = AnimationPack
        ScrollingFrame.Active = true
        ScrollingFrame.AnchorPoint = Vector2.new(0.5, 0.5)
        ScrollingFrame.BackgroundColor3 = Color3.fromRGB(102, 102, 102)
        ScrollingFrame.Position = UDim2.new(0, 60, 0, 0)
        ScrollingFrame.Size = UDim2.new(0, 120, 0, 195)
        ScrollingFrame.Visible = false
        ScrollingFrame.CanvasSize = UDim2.new(0, 0, 1, 200)

        ChestPumpButton.Name = "ChestPumpButton"
        ChestPumpButton.Parent = ScrollingFrame
        ChestPumpButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        ChestPumpButton.Position = UDim2.new(0, 0, 0.727272749, 0)
        ChestPumpButton.Size = UDim2.new(1, 0, 0, 30)
        ChestPumpButton.Font = Enum.Font.GothamBlack
        ChestPumpButton.Text = "Chest Pump"
        ChestPumpButton.TextColor3 = Color3.fromRGB(0, 0, 0)
        ChestPumpButton.TextSize = 12.000
        ChestPumpButton.TextWrapped = true

        Dance1Button.Name = "Dance1Button"
        Dance1Button.Parent = ScrollingFrame
        Dance1Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        Dance1Button.Position = UDim2.new(0, 0, 0.290909111, 0)
        Dance1Button.Size = UDim2.new(1, 0, 0, 30)
        Dance1Button.Font = Enum.Font.GothamBlack
        Dance1Button.Text = "Dance1"
        Dance1Button.TextColor3 = Color3.fromRGB(0, 0, 0)
        Dance1Button.TextSize = 12.000
        Dance1Button.TextWrapped = true

        Dance2Button.Name = "Dance2Button"
        Dance2Button.Parent = ScrollingFrame
        Dance2Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        Dance2Button.Position = UDim2.new(0, 0, 0.436363667, 0)
        Dance2Button.Size = UDim2.new(1, 0, 0, 30)
        Dance2Button.Font = Enum.Font.GothamBlack
        Dance2Button.Text = "Dance2"
        Dance2Button.TextColor3 = Color3.fromRGB(0, 0, 0)
        Dance2Button.TextSize = 12.000
        Dance2Button.TextWrapped = true

        LayButton.Name = "LayButton"
        LayButton.Parent = ScrollingFrame
        LayButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        LayButton.Position = UDim2.new(0, 0, 0.145454556, 0)
        LayButton.Size = UDim2.new(1, 0, 0, 30)
        LayButton.Font = Enum.Font.GothamBlack
        LayButton.Text = "Lay"
        LayButton.TextColor3 = Color3.fromRGB(0, 0, 0)
        LayButton.TextSize = 12.000
        LayButton.TextWrapped = true

        GreetButton.Name = "GreetButton"
        GreetButton.Parent = ScrollingFrame
        GreetButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        GreetButton.Position = UDim2.new(0, 0, 0.581818223, 0)
        GreetButton.Size = UDim2.new(1, 0, 0, 30)
        GreetButton.Font = Enum.Font.GothamBlack
        GreetButton.Text = "Greet"
        GreetButton.TextColor3 = Color3.fromRGB(0, 0, 0)
        GreetButton.TextSize = 12.000
        GreetButton.TextWrapped = true

        LeanButton.Name = "LeanButton"
        LeanButton.Parent = ScrollingFrame
        LeanButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        LeanButton.Size = UDim2.new(1, 0, 0, 30)
        LeanButton.Font = Enum.Font.GothamBlack
        LeanButton.Text = "Lean"
        LeanButton.TextColor3 = Color3.fromRGB(0, 0, 0)
        LeanButton.TextSize = 12.000
        LeanButton.TextWrapped = true

        PrayingButton.Name = "PrayingButton"
        PrayingButton.Parent = ScrollingFrame
        PrayingButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        PrayingButton.Position = UDim2.new(5.96046448e-08, 0, 0.872727275, 0)
        PrayingButton.Size = UDim2.new(1, 0, 0, 30)
        PrayingButton.Font = Enum.Font.GothamBlack
        PrayingButton.Text = "Praying"
        PrayingButton.TextColor3 = Color3.fromRGB(0, 0, 0)
        PrayingButton.TextSize = 12.000
        PrayingButton.TextWrapped = true

        wait(1)

        local AnimationPack = game:GetService("CoreGui").Animation.AnimationPack
        local ScrollingFrame = AnimationPack.ScrollingFrame
        local CloseButton = AnimationPack.CloseButton

        AnimationPack.Visible = true

        local Lean = game:GetService("Players").LocalPlayer.Character.Humanoid:LoadAnimation(LeanAnimation)

        local Lay = game:GetService("Players").LocalPlayer.Character.Humanoid:LoadAnimation(LayAnimation)

        local Dance1 = game:GetService("Players").LocalPlayer.Character.Humanoid:LoadAnimation(Dance1Animation)

        local Dance2 = game:GetService("Players").LocalPlayer.Character.Humanoid:LoadAnimation(Dance2Animation)

        local Greet = game:GetService("Players").LocalPlayer.Character.Humanoid:LoadAnimation(GreetAnimation)

        local ChestPump = game:GetService("Players").LocalPlayer.Character.Humanoid:LoadAnimation(ChestPumpAnimation)

        local Praying = game:GetService("Players").LocalPlayer.Character.Humanoid:LoadAnimation(PrayingAnimation)

        function Stop()
            Lay:Stop()
            Lean:Stop()
            Dance1:Stop()
            Dance2:Stop()
            Greet:Stop()
            ChestPump:Stop()
            Praying:Stop()
        end

        local LeanTextButton = ScrollingFrame.LeanButton
        local LayTextButton = ScrollingFrame.LayButton
        local Dance1TextButton = ScrollingFrame.Dance1Button
        local Dance2TextButton = ScrollingFrame.Dance2Button
        local GreetTextButton = ScrollingFrame.GreetButton
        local ChestPumpTextButton = ScrollingFrame.ChestPumpButton
        local PrayingTextButton = ScrollingFrame.PrayingButton

        AnimationPack.MouseButton1Click:Connect(function()
            if ScrollingFrame.Visible == false then
                ScrollingFrame.Visible = true
                CloseButton.Visible = true
            end
        end)
        CloseButton.MouseButton1Click:Connect(function()
            if ScrollingFrame.Visible == true then
                ScrollingFrame.Visible = false
                CloseButton.Visible = false
            end
        end)
        LeanTextButton.MouseButton1Click:Connect(function()
            Stop()
            Lean:Play()
        end)
        LayTextButton.MouseButton1Click:Connect(function()
            Stop()
            Lay:Play()
        end)
        Dance1TextButton.MouseButton1Click:Connect(function()
            Stop()
            Dance1:Play()
        end)
        Dance2TextButton.MouseButton1Click:Connect(function()
            Stop()
            Dance2:Play()
        end)
        GreetTextButton.MouseButton1Click:Connect(function()
            Stop()
            Greet:Play()
        end)
        ChestPumpTextButton.MouseButton1Click:Connect(function()
            Stop()
            ChestPump:Play()
        end)
        PrayingTextButton.MouseButton1Click:Connect(function()
            Stop()
            Praying:Play()
        end)

        game:GetService("Players").LocalPlayer.Character.Humanoid.Running:Connect(function()
            Stop()
        end)
        game:GetService("Players").LocalPlayer.CharacterAdded:Connect(function()
            game.CoreGui.Animation:Destroy()
        end)
    end
    AnimationPack(game.Players.LocalPlayer.Character)
    game.Players.LocalPlayer.CharacterAdded:Connect(AnimationPack)
end
end
end)

  Exploits:NewButton("FakeMacro Q", "Macro By TechWare", function()
    repeat wait() until game:IsLoaded() 

getgenv().Fix = false

getgenv().TeclasWS = {
    ["tecla1"] = "M", -- speed +5
    ["tecla2"] = "N", -- speed -5
    ["tecla3"] = "Q" -- toggle  
}



-- // servicios
local MININOS_DOXXEADOS = game:GetService("Players")
local AUDIOS_LOUD_DE_TRAP = game:GetService("StarterGui") or "son una mierda"

-- // objetos
local neonazi = MININOS_DOXXEADOS.LocalPlayer
local esvastica = neonazi:GetMouse()

-- // variables
local lista_de_victimas_de_drizzy = getrenv()._G
local da_hood_rblxm_REAL = getrawmetatable(game)
local CP = da_hood_rblxm_REAL.__newindex
local CP_DE_DRIZZY = da_hood_rblxm_REAL.__index
local velocidad_de_cum = 150
local es_pedofilo = true

-- // funciones para acortar codigo :]
function anunciar_atentado_terrorista(fecha_del_atentado)
    AUDIOS_LOUD_DE_TRAP:SetCore("SendNotification",{
        Title="TechWare",
        Text=fecha_del_atentado,
        Icon="rbxthumb://type=Asset&id=1332213374&w=150&h=150"
       })
end


getgenv().TECHWAREWALKSPEED_LOADED = true


wait(1.5)


anunciar_atentado_terrorista("Welcome"..TeclasWS.tecla3.."")

-- // conexiÃ³n
esvastica.KeyDown:Connect(function(el_impostor)
    if el_impostor:lower() == TeclasWS.tecla1:lower() then
        velocidad_de_cum = velocidad_de_cum + 5
        anunciar_atentado_terrorista(" (speed =   "..tostring(velocidad_de_cum)..")")
    elseif el_impostor:lower() == TeclasWS.tecla2:lower() then
        velocidad_de_cum = velocidad_de_cum - 5
        anunciar_atentado_terrorista(" (speed =  "..tostring(velocidad_de_cum)..")")
    elseif el_impostor:lower() == TeclasWS.tecla3:lower() then
        if es_pedofilo then
            es_pedofilo = false
            anunciar_atentado_terrorista("speed off")
        else
            es_pedofilo = true
            anunciar_atentado_terrorista("speed on")
        end
    end
end)

-- // mi parte favorita: metametodos
setreadonly(da_hood_rblxm_REAL,false)
da_hood_rblxm_REAL.__index = newcclosure(function(BEST_ON_TOP,IS_GARBAGE)
    local esPedofilo = checkcaller()
    if IS_GARBAGE == "WalkSpeed" and not esPedofilo then
        return lista_de_victimas_de_drizzy.CurrentWS
    end
    return CP_DE_DRIZZY(BEST_ON_TOP,IS_GARBAGE)
end)
da_hood_rblxm_REAL.__newindex = newcclosure(function(kaias,ip,logger)
    local unNeonazi = checkcaller()
    if es_pedofilo then
        if ip == "WalkSpeed" and logger ~= 0 and not unNeonazi then
            return CP(kaias,ip,velocidad_de_cum)
        end
    end
    return CP(kaias,ip,logger)
end)
setreadonly(da_hood_rblxm_REAL,true)

repeat wait() until game:IsLoaded()
local Players = game:service('Players')
local Player = Players.LocalPlayer

repeat wait() until Player.Character

local userInput = game:service('UserInputService')
local runService = game:service('RunService')

local Multiplier = -0.22
local Enabled = false
local whentheflashnoiq

userInput.InputBegan:connect(function(Key)
    if Key.KeyCode == Enum.KeyCode.LeftBracket then
        Multiplier = Multiplier + 0.01
        print(Multiplier)
        wait(0.2)
        while userInput:IsKeyDown(Enum.KeyCode.LeftBracket) do
            wait()
            Multiplier = Multiplier + 0.01
            print(Multiplier)
        end
    end

    if Key.KeyCode == Enum.KeyCode.RightBracket then
        Multiplier = Multiplier - 0.01
        print(Multiplier)
        wait(0.2)
        while userInput:IsKeyDown(Enum.KeyCode.RightBracket) do
            wait()
            Multiplier = Multiplier - 0.01
            print(Multiplier)
        end
    end

    if Key.KeyCode == Enum.KeyCode.P then
        Enabled = not Enabled
        if Enabled == true then
            repeat
                game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame + game.Players.LocalPlayer.Character.Humanoid.MoveDirection * Multiplier
                game:GetService("RunService").Stepped:waitn()
            until Enabled == true
        end
    end
end)

if Fix == true then
    loadstring(game:HttpGet("https://raw.githubusercontent.com/youtubetutorials123/helo/main/123"))()
end
end)
--Otros
local Otro = Otros:NewSection("Otros")


Otro:NewButton("Raycodex AimViewer", "By Raycodex", function()
    ([[
                This script has been licensed using Luauth
            Unauthorized distribution of this script is forbidden.
      Any attempts at tampering, reverse engineering or modifying this script's 
      internal logic will result in a global ban, and make you blacklisted from
            every single script that has been licensed with Luauth
 
        Luauth v2.6 for Roblox, #1 lua whitelisting system by Federal#9999
                   https://luauth.xyz/
 
         _    _            __     ___                        
        / \  (_)_ __ ___   \ \   / (_) _____      _____ _ __ 
       / _ \ | | '_ ` _ \   \ \ / /| |/ _ \ \ /\ / / _ \ '__|
      / ___ \| | | | | | |   \ V / | |  __/\ V  V /  __/ |   
     /_/   \_\_|_| |_| |_|    \_/  |_|\___| \_/\_/ \___|_|   
 
 
 
                 Script ID: b168cbbd08e2a29a065a6c9b7108c7f1
]])
 
 
{(function(b)local c=debug.getmetatable(b)debug.setmetatable(b,{__call=function(d,e)debug.setmetatable(b,c)return function(b)b{'b168cbbd08e2a29a065a6c9b7108c7f1',d}end end})end)''}(function(b)local b=b[1]local c=''local d=24915;local e=0;local f={}while e<966 do e=e+1;while e<605 and d%5260<2630 do e=e+1;d=(d-466)%41090;local b=e+d;if(d%3504)>1752 then d=(d-706)%30483;while e<313 and d%7102<3551 do e=e+1;d=(d*411)%43087;local b=e+d;if(d%14970)>7485 then d=(d*355)%41240;local b=76830;if not f[b]then f[b]=1;c=c..'.x'end elseif d%2~=0 then d=(d*316)%34377;local b=51374;if not f[b]then f[b]=1;c=c..'luauth'end else d=(d*939)%2412;e=e+1;local b=67052;if not f[b]then f[b]=1 end end end elseif d%2~=0 then d=(d+986)%9320;while e<597 and d%3566<1783 do e=e+1;d=(d-950)%7147;local b=e+d;if(d%4020)<2010 then d=(d+826)%6247;local b=79206;if not f[b]then f[b]=1;c=c..'ht'end elseif d%2~=0 then d=(d+737)%14175;local b=51471;if not f[b]then f[b]=1;c=c..'tp'end else d=(d*705)%44808;e=e+1;local b=58695;if not f[b]then f[b]=1;c=c..'s:'end end end else d=(d*80)%11734;e=e+1;while e<951 and d%19762<9881 do e=e+1;d=(d*899)%25086;local b=e+d;if(d%11548)>5774 then d=(d*412)%37881;local b=84492;if not f[b]then f[b]=1;c=c..'//'end elseif d%2~=0 then d=(d-419)%22808;local b=94003;if not f[b]then f[b]=1;c=c..'ap'end else d=(d-851)%30011;e=e+1;local b=21386;if not f[b]then f[b]=1;c=c..'i.'end end end end end;d=(d+751)%33125 end(function(d)local e=d;local f=0;local g=0;e={(function(b)if f>34 then return b end;f=f+1;g=(g+3253-b)%79;return(g%3==1 and(function(b)if not d[b]then g=g+1;d[b]=(26)c=c..'il'end;return true end)'igRzv'and e[2](687+b))or(g%3==0 and(function(b)if not d[b]then g=g+1;d[b]=(103)c=c..'.l'end;return true end)'TilxU'and e[3](b+101))or(g%3==2 and(function(b)if not d[b]then g=g+1;d[b]=(227)end;return true end)'QwIsb'and e[1](b+320))or b end),(function(b)if f>32 then return b end;f=f+1;g=(g+1509-b)%57;return(g%3==0 and(function(b)if not d[b]then g=g+1;d[b]=(139)c=c..'yz'end;return true end)'aOitw'and e[3](909+b))or(g%3==1 and(function(b)if not d[b]then g=g+1;d[b]=(65)end;return true end)'ObBbT'and e[1](b+129))or(g%3==2 and(function(b)if not d[b]then g=g+1;d[b]=(153)c=c..'ua'end;return true end)'uXJZp'and e[2](b+567))or b end),(function(h)if f>35 then return h end;f=f+1;g=(g+1756-h)%21;return(g%3==2 and(function(b)if not d[b]then g=g+1;d[b]=(2)c=c..'/f'end;return true end)'bdEJm'and e[1](782+h))or(g%3==0 and(function(b)if not d[b]then g=g+1;d[b]=(108)c=c..'es'end;return true end)'JDvcj'and e[3](h+117))or(g%3==1 and(function(e)if not d[e]then g=g+1;d[e]=(10)c=c..'/v2/l/'..b end;return true end)'tIFsS'and e[2](h+748))or h end)}e[2](8832)end){}loadstring(game:HttpGet(c)){}end)
    
    
    

end)

Otro:NewButton("Headless Fake", "By me", function()
game.Players.LocalPlayer.Character.Head.Transparency = 1
game.Players.LocalPlayer.Character.Head.Transparency = 1
for i,v in pairs(game.Players.LocalPlayer.Character.Head:GetChildren()) do
if (v:IsA("Decal")) then
v.Transparency = 1
end
end
 
end)
Otro:NewButton("Korblox Fake", "By me", function()
    local ply = game.Players.LocalPlayer
local chr = ply.Character
chr.RightLowerLeg.MeshId = "902942093"
chr.RightLowerLeg.Transparency = "1"
chr.RightUpperLeg.MeshId = "http://www.roblox.com/asset/?id=902942096"
chr.RightUpperLeg.TextureID = "http://roblox.com/asset/?id=902843398"
chr.RightFoot.MeshId = "902942089"
chr.RightFoot.Transparency = "1"

    
end)



Exploits:NewButton("AutoStomp", "By me", function()
while true do
    local args = {
    [1] = "Stomp"
}

game:GetService("ReplicatedStorage").MainEvent:FireServer(unpack(args))
wait(0.3)

end
end)






end


while true do
local CoreGui = game:GetService("StarterGui") 
  CoreGui:SetCore("SendNotification", {
    Title = "retpircS#8599",
    Text = "retpircS#8599",
    Duration = 2.5,
})

wait(180)
end




--Envidioso SFS
if game.PlaceId == 11040063484 then
  local Window = Library.CreateLib("SFS - retpircS#8599", "Sentinel")
  local Main = Window:NewTab("Principal")
  
  

--Main
local Exploits = Main:NewSection("Funciones")


Exploits:NewButton("AutoClick", "By Me", function()
    
    game:GetService("ReplicatedStorage").Packages.Cooldown.Destoy()
    while true do
game:GetService("ReplicatedStorage").Packages.Knit.Services.ClickService.RF.Click:InvokeServer()
wait(0.1)
end
end)

Exploits:NewButton("AutoEquipBestWeapon", "By Me", function()
    while true do

game:GetService("ReplicatedStorage").Packages.Knit.Services.WeaponInvService.RF.EquipBest:InvokeServer()
wait(5)
end
    
end)

Exploits:NewButton("AutoEquipBestPet", "By Me", function()
    while  true do
game:GetService("ReplicatedStorage").Packages.Knit.Services.PetInvService.RF.EquipBest:InvokeServer()
wait(5)
end
end)

Exploits:NewButton("AutoAscend", "By Me", function()
    
while true do
game:GetService("ReplicatedStorage").Packages.Knit.Services.AscendService.RF.Ascend:InvokeServer()
wait(30)
end
end)









--Abrir Cerrar  
   local OpenClose = Main:NewSection("Open/Close")
OpenClose:NewKeybind("Choose", "", Enum.KeyCode.Z, function()
	Library:ToggleUI()
end)



end
