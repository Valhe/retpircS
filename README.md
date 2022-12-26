loadstring(game:HttpGet("https://raw.githubusercontent.com/Valhe/DhAimTrainner/main/README.md "))()

--Envidioso SFS

spawn(function() 
if game.PlaceId == 11040063484 then
  local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
  local Window = Library.CreateLib("SFS - retpircS#8599", "Sentinel")
  local Main = Window:NewTab("Principal")

--Main
local Exploits = Main:NewSection("Funciones")

Exploits:NewButton("AutoClick", "By Me", function()
   while true do
   game:GetService("ReplicatedStorage").Packages.Knit.Services.ClickService.RF.Click:InvokeServer()
   wait(0.2)
   end
end)



Exploits:NewButton("AutoEquipBestWeapon", "By Me", function()
   while true do
   game:GetService("ReplicatedStorage").Packages.Knit.Services.WeaponInvService.RF.EquipBest:InvokeServer()
   wait(5)
   end
end)

Exploits:NewButton("AutoEquipBestPet", "By Me", function()
    while true do
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
end)
