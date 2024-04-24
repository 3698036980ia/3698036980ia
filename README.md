local player = game.Players.LocalPlayer
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "JesioScript", HidePremium = false, SaveConfig = true, ConfigFolder = "OrionTest"})

local Tab = Window:MakeTab({
	Name = "Scripts",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddButton({
	Name = "Speed",
	Callback = function()
game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 100
  	end    
})

Tab:AddButton({
	Name = "Infinite yield",
	Callback = function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
  	end    
})

Tab:AddButton({
	Name = "Jump",
	Callback = function()
game.Players.LocalPlayer.Character.Humanoid.JumpPower = 100
  	end    
})

Tab:AddButton({
	Name = "Fly",
	Callback = function()
loadstring(game:HttpGet('https://pastebin.com/raw/YSL3xKYU'))()
  	end    
})

Tab:AddButton({
	Name = "Shift Lock",
	Callback = function()
loadstring(game:HttpGet('https://pastebin.com/raw/WQ9NPeDS'))();
  	end    
})

Tab:AddButton({
	Name = "Fling",
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/0Ben1/fe./main/Fling%20GUI"))()
  	end    
})

Tab:AddButton({
	Name = "Fling all",
	Callback = function()
loadstring(game:HttpGet("https://pastebin.com/raw/zqyDSUWX"))()
  	end    
})

Tab:AddButton({
	Name = "Noclip",
	Callback = function()
loadstring(game:HttpGet(("https://pastebin.com/raw/w0XEUW3y"),true))()
  	end    
})

Tab:AddButton({
	Name = "For Noclip",
	Callback = function()
loadstring(game:HttpGet(('https://pastefy.app/Te4dwSw2/raw'),true))()
  	end    
})

Tab:AddButton({
	Name = "AimLock",
	Callback = function()
loadstring(game:HttpGet(("https://pastebin.com/raw/w0XEUW3y"),true))()
  	end    
})


Tab:AddButton({
	Name = "Radio No Fe",
	Callback = function()
G.boomboxb = game:GetObjects('rbxassetid://740618400')[1]
_G.boomboxb.Parent = game:GetService'Players'.LocalPlayer.Backpack
loadstring(_G.boomboxb.Client.Source)() 
loadstring(_G.boomboxb.Server.Source)()
	end    
})



local Tab = Window:MakeTab({
	Name = "For Games",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddButton({
	Name = "Murder Mystery 2",
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/Gregory909/FolderGui-FolderHub/main/loader.lua", true))()
  	end    
})

Tab:AddButton({
	Name = "Muscle Legeng",
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/AliCode14/scripts/main/ScriptHub.lua"))()
  	end    
})

Tab:AddButton({
	Name = "Da Hood",
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/jemangeleZ/KLD/main/KLD", true))()
  	end    
})

Tab:AddButton({
	Name = "Pet Simulator X",
	Callback = function()
loadstring(game:HttpGet(('https://raw.githubusercontent.com/rblxscriptsnet/unfair/main/rblxhub.lua'),true))()
  	end    
})

Tab:AddButton({
	Name = "Murder Mystery 2",
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/KINGHUB01/BlackKing/main/BlackKing"))()
  	end    
})

Tab:AddButton({
	Name = "ragdoll enigne",
	Callback = function()
loadstring(game:HttpGet(('https://raw.githubusercontent.com/ggshizuru/myScriptHub/main/ShizzuruHub.1.lua'),true))()
  	end    
})

Tab:AddButton({
	Name = "Brookhaven",
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/IceMael7/NewIceHub/main/Brookhaven"))()
  	end    
})

Tab:AddButton({
	Name = "Murder Mystery 2 (My script)",
	Callback = function()
loadstring(game:HttpGet(("https://pastefy.app/CxrysIi5/raw"),true))()
  	end    
})

Tab:AddButton({
	Name = "OMG Blox Fruits",
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/Omgshit/Scripts/main/MainLoader.lua"))()
  	end    
})

Tab:AddButton({
	Name = "Redz999 Blox Fruits",
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/REDzHUB/BloxFruits/main/redz9999"))()
  	end    
})
   

local Tab = Window:MakeTab({
	Name = "Fe Script",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local Section = Tab:AddSection({
	Name = "Fe Script"
})

Tab:AddButton({
	Name = "Fe Animation",
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/GamingScripter/Animation-Hub/main/Animation%20Gui", true))()
  	end    
})

Tab:AddButton({
	Name = "No Fe Headless",
	Callback = function()
		local lp = game:GetService "Players".LocalPlayer
		if lp.Character:FindFirstChild "Head" then
			local char = lp.Character
			char.Archivable = true
			local new = char:Clone()
			new.Parent = workspace
			lp.Character = new
			wait(2)
			local oldhum = char:FindFirstChildWhichIsA "Humanoid"
			local newhum = oldhum:Clone()
			newhum.Parent = char
			newhum.RequiresNeck = false
			oldhum.Parent = nil
			wait(2)
			lp.Character = char
			new:Destroy()
			wait(1)
			newhum:GetPropertyChangedSignal("Health"):Connect(
				function()
					if newhum.Health <= 0 then
						oldhum.Parent = lp.Character
						wait(1)
						oldhum:Destroy()
					end
				end)
			workspace.CurrentCamera.CameraSubject = char
			if char:FindFirstChild "Animate" then
				char.Animate.Disabled = true
				wait(.1)
				char.Animate.Disabled = false
			end
			lp.Character:FindFirstChild "Head":Destroy()
		end
  	end    
})

local Tab = Window:MakeTab({
	Name = "ScriptHub",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local Section = Tab:AddSection({
	Name = "ScriptHub"
})

Tab:AddButton({
	Name = "Avtor Script Hub",
	Callback = function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/Avtor1zaTion/Avtor/main/AvtorHub'))()
  	end    
})

Tab:AddButton({
	Name = "Winter Hub For Blox Fruits",
	Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/Yatsuraa/Yuri/main/Winterhub_V2.lua"))("t.me/arceusxscripts")
  	end    
})

Tab:AddButton({
	Name = "Suslik Hub",
	Callback = function()
loadstring(game:HttpGet"https://raw.githubusercontent.com/KrutoySuslik/-SuslikHub-/main/%7CSuslik%20Hub%7C%20%7CAll%20Scripts%7C")("https://t.me/arceusxscripts")
  	end    
})

Tab:AddButton({
	Name = "Ghost Hub",
	Callback = function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()
  	end    
})

Tab:AddButton({
	Name = "Equinox hub",
	Callback = function()
loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
  	end    
})

local Tab = Window:MakeTab({
	Name = "Creator:",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddButton({
	Name = "Nick x1keng",
	Callback = function()
loadstring(game:HttpGet("https://pastebin.com/raw/zqyDSUWX"))()
  	end    
})

Tab:AddButton({
	Name = "Telegram channel @jesioscript",
	Callback = function()
loadstring(game:HttpGet("https://pastebin.com/raw/zqyDSUWX"))()
  	end    
}) 
