local OrionLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/shlexware/Orion/main/source"))()


local Window = OrionLib:MakeWindow({Name = "人机还用外挂", HidePremium = false, SaveConfig = false, IntroText = "人机", ConfigFolder = "人机"})

OrionLib:MakeNotification({
	Name = "欢迎人机龙脚本",
	Content =  "当前游戏ID为:" .. game.GameId .. ".",
	Image = "rbxassetid://7734068321",
	Time = 5
})


local Tab = Window:MakeTab({
	Name = "ud有话说",
	Icon = "rbxassetid://7734068321",
	PremiumOnly = false
})

Tab:AddParagraph("你就是个人机","你就是个傻逼")

Tab:AddParagraph("温馨提示","不要忘记你是个傻逼，人机（作者3077301487）")

local Tab = Window:MakeTab({
	Name = "极速传奇",
	Icon = "rbxassetid://7734068321",
	PremiumOnly = false
})



local Section = Tab:AddSection({
	Name = "功能"
})



Tab:AddButton({
	Name = "开启卡宠",
	Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/cbhlyy/lyycbh/main/jisu1"))()		
  	end
})


Tab:AddButton({
	Name = "自动重生和自动刷等级",
	Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/cbhlyy/lyycbh/main/jusu2"))()        
  	end    
})

Tab:AddButton({
	Name = "反挂机【防检测】",
	Callback = function()
		print("Anti Afk On")
		local vu = game:GetService("VirtualUser")
		game:GetService("Players").LocalPlayer.Idled:connect(function()
		   vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
		   wait(1)
		   vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
		end)
  	end    
})

local Section = Tab:AddSection({
	Name = "传送岛屿"
})

Tab:AddButton({
	Name = "返还出生岛",
	Callback = function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-9682.98828125, 58.87917709350586, 3099.033935546875)      
  	end    
})

Tab:AddButton({
	Name = "白雪城",
	Callback = function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-9676.138671875, 58.87917709350586, 3782.69384765625)   
  	end    
})

Tab:AddButton({
	Name = "熔岩城",
	Callback = function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-11054.96875, 216.83917236328125, 4898.62841796875)       
  	end    
})

Tab:AddButton({
	Name = "传奇公路",
	Callback = function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-13098.87109375, 216.83917236328125, 5907.6279296875)    
  	end    
})

local Tab = Window:MakeTab({
	Name = "造船寻宝",
	Icon = "rbxassetid://7734068321",
	PremiumOnly = false
})



local Section = Tab:AddSection({
	Name = "功能"
})




Tab:AddButton({
	Name = "自动刷金条",
	Callback = function()
	loadstring(game:HttpGet("https://raw.githubusercontent.com/cbhlyy/lyycbh/main/zaochuan1"))()
  	end
})

Tab:AddButton({
	Name = "工具包（可破别人团队模式空气墙）",
	Callback = function()
	loadstring(game:HttpGet("https://cdn.wearedevs.net/scripts/BTools.txt"))()	
  	end
})

Tab:AddButton({
	Name = "普通飞行",
	Callback = function()
	loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\40\39\104\116\116\112\115\58\47\47\103\105\115\116\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\109\101\111\122\111\110\101\89\84\47\98\102\48\51\55\100\102\102\57\102\48\97\55\48\48\49\55\51\48\52\100\100\100\54\55\102\100\99\100\51\55\48\47\114\97\119\47\101\49\52\101\55\52\102\52\50\53\98\48\54\48\100\102\53\50\51\51\52\51\99\102\51\48\98\55\56\55\48\55\52\101\98\51\99\53\100\50\47\97\114\99\101\117\115\37\50\53\50\48\120\37\50\53\50\48\102\108\121\37\50\53\50\48\50\37\50\53\50\48\111\98\102\108\117\99\97\116\111\114\39\41\44\116\114\117\101\41\41\40\41\10\10")()
  	end
})
