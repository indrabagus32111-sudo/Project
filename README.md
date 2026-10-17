-- This File Was Deobfuscated In Null
-- discord.gg/M9Tm9RT7ta

local tweenService = game:GetService("TweenService")
local coreGui = game:GetService("CoreGui")
local players = game:GetService("Players")
local runService = game:GetService("RunService")
local userInputService = game:GetService("UserInputService")
local lighting = game:GetService("Lighting")
local replicatedStorage = game:GetService("ReplicatedStorage")
local workspaceService = game:GetService("Workspace")
local guiService = game:GetService("GuiService")
local virtualInputManager = game:GetService("VirtualInputManager")
local collectionService = game:GetService("CollectionService")
local httpService = game:GetService("HttpService")
local teams = game:GetService("Teams")

local v1 = getgenv()

v1.VD = getgenv().VD or {
  AutoSkillcheck = false,
  AutoSkillcheckMode = "Normal",
  SURV_FleeKiller = false,
  SURV_FleeDistance = 40,
  SURV_AutoParry = false,
  SURV_ParryMode = "Legit",
  SURV_ParryAnimId = "rbxassetid://109133187196613",
  SURV_ParryRange = 12,
  SURV_ShowParryCircle = true,
  Parry_Keybind = "F3",
  SURV_AntiKnock = false,
  SURV_FirstPerson = false,
  AUTO_ToFAim = false,
  AUTO_ToFAimRange = 90,
  AUTO_ToFDotThreshold = 0.5,
  AUTO_ToFTargetMode = "Killer",
  AUTO_ToFAimPart = "HumanoidRootPart",
  AUTO_ToFPredict = true,
  AUTO_ToFBulletSpeed = 200,
  AUTO_Attack = false,
  AUTO_AttackRange = 12,
  KILLER_DestroyPallets = false,
  KILLER_AutoBreakGene = false,
  KILLER_BlockVaults = false,
  KILLER_AntiBlind = false,
  KILLER_DoubleTap = false,
  SPEAR_Aimbot = false,
  SPEAR_Gravity = 50,
  SPEAR_Speed = 100,
  KILLER_CustomMasked = "Richard",
  DRAWING_ESP = false,
  ESP_Skeleton = false,
  ESP_Offscreen = false,
  ESP_Velocity = false,
  MaxDistance = 2000,
  InstantHealSelf = false,
  AutoHealAll = false,
  Destroyed = false,
  SURV_GenBoost = false,
  SURV_DraggableGenBypass = false,
  ESP_LowPerformance = false,
  Fullbright = false,
  NoFog = false,
  SURV_AutoDropPallet = false,
  SURV_AutoDropPalletDist = 20,
  SURV_AutoDropPalletMode = "Aggressive",
  SURV_AutoVault = false,
  SURV_AutoPalletSlide = false,
}

local function f1()
  return gethui and gethui() or coreGui
end

local function f2()
  local parent = f1()

  local noMercyWelcome = Instance.new("ScreenGui")
  noMercyWelcome.Name = "NoMercyWelcome"
  noMercyWelcome.ResetOnSpawn = false
  noMercyWelcome.IgnoreGuiInset = true
  noMercyWelcome.ZIndexBehavior = Enum.ZIndexBehavior.Global
  noMercyWelcome.Parent = parent

  if syn and syn.protect_gui then
    pcall(syn.protect_gui, noMercyWelcome)
  end

  local frame = Instance.new("Frame")
  frame.Size = UDim2.fromOffset(260, 260)
  frame.Position = UDim2.new(0.5, 0, 0.5, 0)
  frame.AnchorPoint = Vector2.new(0.5, 0.5)
  frame.BackgroundTransparency = 1
  frame.ZIndex = 999
  frame.Parent = noMercyWelcome

  local imageLabel = Instance.new("ImageLabel")
  imageLabel.Size = UDim2.fromOffset(0, 0)
  imageLabel.Position = UDim2.new(0.5, 0, 0.4, 0)
  imageLabel.AnchorPoint = Vector2.new(0.5, 0.5)
  imageLabel.Image = "rbxassetid://113381647185328"
  imageLabel.BackgroundTransparency = 1
  imageLabel.ZIndex = 999
  imageLabel.Parent = frame

  local uiCorner = Instance.new("UICorner")
  uiCorner.CornerRadius = UDim.new(1, 0)
  uiCorner.Parent = imageLabel

  local uiStroke = Instance.new("UIStroke")
  uiStroke.Color = Color3.fromRGB(255, 255, 255)
  uiStroke.Thickness = 4
  uiStroke.Transparency = 1
  uiStroke.Parent = imageLabel

  local textLabel = Instance.new("TextLabel")
  textLabel.Size = UDim2.new(1, 0, 0, 40)
  textLabel.Position = UDim2.new(0.5, 0, 0.75, 0)
  textLabel.AnchorPoint = Vector2.new(0.5, 0)
  textLabel.BackgroundTransparency = 1
  textLabel.Text = "WELCOME A2"
  textLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
  textLabel.TextSize = 18
  textLabel.Font = Enum.Font.GothamBold
  textLabel.TextTransparency = 1
  textLabel.ZIndex = 999
  textLabel.Parent = frame

  local create = tweenService:Create(imageLabel, TweenInfo.new(
    0.6, Enum.EasingStyle.Back, Enum.EasingDirection.Out
  ), { Size = UDim2.fromOffset(150, 150) })

  local create2 = tweenService:Create(uiStroke, TweenInfo.new(0.4), { Transparency = 0 })
  local create3 = tweenService:Create(textLabel, TweenInfo.new(0.4), { TextTransparency = 0 })
  create:Play()
  create2:Play()
  create3:Play()
  create.Completed:Wait()
  local v2 = true

  task.spawn(function()
    while v2 do
      local create4 = tweenService:Create(uiStroke, TweenInfo.new(
        0.6, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut
      ), { Transparency = 0.8, Thickness = 6 })

      create4:Play()
      create4.Completed:Wait()

      if not v2 then
        break
      else
        local create5 = tweenService:Create(uiStroke, TweenInfo.new(
          0.6, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut
        ), { Transparency = 0, Thickness = 2 })

        create5:Play()
        create5.Completed:Wait()
      end
    end
  end)

  task.wait(1.5)

  v2 = false

  local create6 = tweenService:Create(imageLabel, TweenInfo.new(
    0.4, Enum.EasingStyle.Quad, Enum.EasingDirection.In
  ), { Size = UDim2.fromOffset(0, 0) })

  local create7 = tweenService:Create(uiStroke, TweenInfo.new(0.3), { Transparency = 1 })
  local create8 = tweenService:Create(textLabel, TweenInfo.new(0.3), { TextTransparency = 1 })
  create6:Play()
  create7:Play()
  create8:Play()
  create6.Completed:Wait()
  noMercyWelcome:Destroy()
end

if pcall(function()
  local v3 = loadstring((game:HttpGet("https://raw.githubusercontent.com/aseumusu-design/NoMercy_BladeBal/refs/heads/main/intro.lua")))

  if v3 then
    v3()
  end
end) then
  task.wait(6.5)
else
  f2()
end

local uiLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/Marpiii/UiLib/refs/heads/main/source.lua"))()
local f3

local window = uiLib:MakeWindow({
  Name = "A2 — VIOLENCE DISTRICT",
  HidePremium = false,
  SaveConfig = true,
  ConfigFolder = "NoMercyViolenceFullZiaan",
  IntroEnabled = false,
  Icon = "rbxassetid://113381647185328",
  CloseCallback = function()
    if f3 then
      f3()
    end
  end,
})

local function f4()
  local v4 = f1()

  if not v4 then
    return nil
  else
    local marV = v4:FindFirstChild("MarV")

    if not marV then
      return nil
    end

    for index, value in ipairs(marV:GetChildren()) do
      if value:IsA("Frame") and value.AbsoluteSize.X > 300 then
        return value
      end
    end

    return nil
  end
end

local v5 = nil

local function f5()
  if v5 then
    v5:Destroy()
  end

  local noMercyBubble = Instance.new("ScreenGui")
  noMercyBubble.Name = "NoMercyBubble"
  noMercyBubble.ResetOnSpawn = false
  noMercyBubble.IgnoreGuiInset = true
  noMercyBubble.ZIndexBehavior = Enum.ZIndexBehavior.Global
  noMercyBubble.Parent = f1()

  if syn and syn.protect_gui then
    pcall(syn.protect_gui, noMercyBubble)
  end

  local imageButton = Instance.new("ImageButton")
  imageButton.Parent = noMercyBubble
  imageButton.BackgroundColor3 = Color3.fromRGB(25, 30, 35)
  imageButton.Position = UDim2.new(0.02, 0, 0.2, 0)
  imageButton.Size = UDim2.fromOffset(48, 48)
  imageButton.Image = "rbxassetid://113381647185328"
  imageButton.ScaleType = Enum.ScaleType.Fit
  imageButton.Active = true
  imageButton.Draggable = true
  imageButton.ZIndex = 10

  local uiCorner2 = Instance.new("UICorner")
  uiCorner2.CornerRadius = UDim.new(0, 10)
  uiCorner2.Parent = imageButton

  local uiStroke2 = Instance.new("UIStroke")
  uiStroke2.Color = Color3.fromRGB(255, 255, 255)
  uiStroke2.Thickness = 2
  uiStroke2.Transparency = 0
  uiStroke2.Parent = imageButton

  local v6 = true

  task.spawn(function()
    while v6 and uiStroke2 and uiStroke2.Parent do
      local create9 = tweenService:Create(uiStroke2, TweenInfo.new(
        0.8, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut
      ), { Transparency = 0.8, Thickness = 4 })

      create9:Play()
      create9.Completed:Wait()

      if not v6 or not uiStroke2 or not uiStroke2.Parent then
        break
      else
        local create10 = tweenService:Create(uiStroke2, TweenInfo.new(
          0.8, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut
        ), { Transparency = 0, Thickness = 2 })

        create10:Play()
        create10.Completed:Wait()
      end
    end
  end)

  imageButton.MouseButton1Click:Connect(function()
    v6 = false
    local v7 = f4()

    if v7 then
      v7.Visible = true
    end

    v5:Destroy()
    v5 = nil
  end)

  v5 = noMercyBubble
end

local function f6()
  local v8 = f4()

  if v8 then
    v8.Visible = true
  end
end

local function f7()
  local v9 = f4()

  if v9 then
    v9.Visible = false
  end

  f5()
end

local function f8(p1)
  if p1 then
    f6()
  end

  local parent2 = f1()

  local noMercyConfirm = Instance.new("ScreenGui")
  noMercyConfirm.Name = "NoMercyConfirm"
  noMercyConfirm.ResetOnSpawn = false
  noMercyConfirm.IgnoreGuiInset = true
  noMercyConfirm.ZIndexBehavior = Enum.ZIndexBehavior.Global
  noMercyConfirm.Parent = parent2

  if syn and syn.protect_gui then
    pcall(syn.protect_gui, noMercyConfirm)
  end

  local frame2 = Instance.new("Frame")
  frame2.Size = UDim2.new(1, 0, 1, 0)
  frame2.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
  frame2.BackgroundTransparency = 0.4
  frame2.ZIndex = 99
  frame2.Parent = noMercyConfirm

  local frame3 = Instance.new("Frame")
  frame3.Size = UDim2.fromOffset(280, 150)
  frame3.Position = UDim2.new(0.5, 0, 0.5, 0)
  frame3.AnchorPoint = Vector2.new(0.5, 0.5)
  frame3.BackgroundColor3 = Color3.fromRGB(28, 32, 38)
  frame3.BorderSizePixel = 0
  frame3.ZIndex = 100
  frame3.Parent = noMercyConfirm

  local uiCorner3 = Instance.new("UICorner")
  uiCorner3.CornerRadius = UDim.new(0, 12)
  uiCorner3.Parent = frame3

  local textLabel2 = Instance.new("TextLabel")
  textLabel2.Size = UDim2.new(1, -40, 0, 30)
  textLabel2.Position = UDim2.new(0, 20, 0, 15)
  textLabel2.BackgroundTransparency = 1
  textLabel2.Text = "Tutup A2?"
  textLabel2.TextColor3 = Color3.fromRGB(240, 240, 240)
  textLabel2.TextSize = 18
  textLabel2.Font = Enum.Font.GothamBold
  textLabel2.TextXAlignment = Enum.TextXAlignment.Left
  textLabel2.ZIndex = 101
  textLabel2.Parent = frame3

  local textLabel3 = Instance.new("TextLabel")
  textLabel3.Size = UDim2.new(1, -40, 0, 30)
  textLabel3.Position = UDim2.new(0, 20, 0, 48)
  textLabel3.BackgroundTransparency = 1
  textLabel3.Text = "Klik bubble untuk buka lagi."
  textLabel3.TextColor3 = Color3.fromRGB(150, 150, 150)
  textLabel3.TextSize = 14
  textLabel3.Font = Enum.Font.Gotham
  textLabel3.TextXAlignment = Enum.TextXAlignment.Left
  textLabel3.ZIndex = 101
  textLabel3.Parent = frame3

  local function f9()
    noMercyConfirm:Destroy()
  end

  local function f10()
    f9()

    if p1 then
      f6()
    end
  end

  local textButton = Instance.new("TextButton")
  textButton.Size = UDim2.fromOffset(90, 36)
  textButton.Position = UDim2.new(1, -200, 1, -50)
  textButton.BackgroundColor3 = Color3.fromRGB(60, 60, 60)
  textButton.BorderSizePixel = 0
  textButton.Text = "Ya"
  textButton.TextColor3 = Color3.fromRGB(255, 255, 255)
  textButton.TextSize = 15
  textButton.Font = Enum.Font.GothamBold
  textButton.ZIndex = 101
  textButton.Parent = frame3

  local uiCorner4 = Instance.new("UICorner")
  uiCorner4.CornerRadius = UDim.new(0, 8)
  uiCorner4.Parent = textButton

  textButton.MouseButton1Click:Connect(function()
    f9()
    f7()
  end)

  local textButton2 = Instance.new("TextButton")
  textButton2.Size = UDim2.fromOffset(90, 36)
  textButton2.Position = UDim2.new(1, -100, 1, -50)
  textButton2.BackgroundColor3 = Color3.fromRGB(40, 45, 52)
  textButton2.BorderSizePixel = 0
  textButton2.Text = "Tidak"
  textButton2.TextColor3 = Color3.fromRGB(240, 240, 240)
  textButton2.TextSize = 15
  textButton2.Font = Enum.Font.GothamBold
  textButton2.ZIndex = 101
  textButton2.Parent = frame3

  local uiCorner5 = Instance.new("UICorner")
  uiCorner5.CornerRadius = UDim.new(0, 8)
  uiCorner5.Parent = textButton2

  textButton2.MouseButton1Click:Connect(f10)

  frame2.InputBegan:Connect(function(input)
    if input.UserInputType == Enum.UserInputType.MouseButton1 then
      f10()
    end
  end)
end

function f3()
  f8(true)
end

local tentangAddSection = window:MakeTab({
  Name = "Info",
  Icon = "rbxassetid://7733964719",
  PremiumOnly = false,
}):AddSection({
  Name = "Tentang",
})

tentangAddSection:AddLabel("A2 — Violence District")
tentangAddSection:AddLabel("A2 Official Script — Full Mobile Build (Skillcheck & Survivor)")

tentangAddSection:AddButton({
  Name = "Copy Discord",
  Callback = function()
    if setclipboard then
      setclipboard("https://discord.gg/pbg6g79Hp")
    end

    uiLib:MakeNotification({
      Name = "A2",
      Content = "Link Discord di-copy!",
      Image = "rbxassetid://113381647185328",
      Time = 3,
    })
  end,
})

tentangAddSection:AddButton({ Name = "Tutup UI (Close)", Callback = function() f8() end })

local v12 = {
  Survivor = "rbxassetid://7743875962",
}

local v13 = {}

local function f12(p3, p4, p5)
  uiLib:MakeNotification({
    Name = p3 or "A2",
    Content = p4 or "",
    Image = "rbxassetid://113381647185328",
    Time = p5 or 3,
  })
end

local function f13(p6, p7)
  if p6 and p7 then
    v13[p6] = p7
  end
end

local f14

function f14(p8, p9)
  local addSection = p8:AddSection({ Name = p9 or "Menu" })

  local v14 = {}
  v14.__orionTab = p8
  v14.__orionSection = addSection

  function v14:AddSection(p10)
    local name = type(p10) == "table" and p10.Name or tostring(p10 or "")

    if name ~= "" then
      return f14(p8, name)
    end

    return self
  end

  function v14:AddToggle(p13)
    local v16 = p13 or {}
    local flag = v16.Flag or v16.Name
    local addToggle
    pcall(function()
      addToggle = addSection:AddToggle({
        Name = v16.Name or "Toggle",
        Default = v16.Default or false,
        Callback = function(v)
          if v16.Callback then pcall(v16.Callback, v) end
        end
      })
    end)
    f13(flag, addToggle)
    return addToggle
  end

  function v14:AddSlider(p14)
    local v18 = p14 or {}
    local addSlider
    pcall(function()
      addSlider = addSection:AddSlider({
        Name = v18.Name or "Slider",
        Min = v18.Min or 0,
        Max = v18.Max or 100,
        Default = v18.Default or v18.Min or 0,
        Increment = v18.Increment or 1,
        ValueName = v18.Suffix or "",
        Callback = function(value5)
          if v18.Callback then pcall(v18.Callback, value5) end
        end,
      })
    end)
    f13(v18.Flag or v18.Name, addSlider)
    return addSlider
  end

  function v14:AddDropdown(p16)
    local v20 = p16 or {}
    local values = v20.Values or v20.Options or {}
    local addDropdown
    pcall(function()
      addDropdown = addSection:AddDropdown({
        Name = v20.Name or "Dropdown",
        Default = v20.Default or values[1],
        Values = values,
        Callback = function(v)
          if v20.Callback then pcall(v20.Callback, v) end
        end
      })
    end)
    f13(v20.Flag or v20.Name, addDropdown)
    return addDropdown
  end

  function v14:AddCenterTabbox(p23)
    return NM_MakeTabbox(p8, p23)
  end

  return v14
end

function NM_MakeTabbox(p24, p25)
  local v30 = {}
  if p25 and p25 ~= "" then
    pcall(function() p24:AddSection({ Name = tostring(p25) }) end)
  end
  function v30:AddTab(p26)
    return f14(p24, type(p26) == "table" and p26.Name or tostring(p26 or "Tab"))
  end
  return v30
end

local v31 = { ConfigElements = v13 }

function v31:AddTab(p28)
  local name2 = (p28 or {}).Name or "Tab"
  local tab = window:MakeTab({
    Name = name2,
    Icon = v12[name2] or "rbxassetid://7734053495",
    PremiumOnly = false,
  })

  local v33 = {}
  v33.__orionTab = tab

  function v33:AddSection(p29)
    return f14(tab, type(p29) == "table" and p29.Name or tostring(p29 or "Menu"))
  end

  function v33:AddCenterTabbox(p30)
    return NM_MakeTabbox(tab, p30)
  end

  return v33
end

local function f15()
  local localPlayer, currentCamera, touchEnabled, v176
  localPlayer = players.LocalPlayer
  currentCamera = workspaceService.CurrentCamera
  touchEnabled = userInputService.TouchEnabled and not userInputService.KeyboardEnabled

  local playerGui4 = localPlayer:WaitForChild("PlayerGui")

  v176 = {
    LastGoalRotation = nil,
    HasClickedThisGoal = false,
    LastLineRotation = nil,
    LastTick = nil,
    WasActive = false,
    PerfectLastGoalRotation = nil,
    PerfectHasClickedThisGoal = nil,
    InstantLastTriggerTick = 0,
    InstantLastGoalRotation = 0,
    InstantLastGoalInstance = nil,
    InstantCurrentGoalID = 0,
    InstantHasClicked = false,
    InstantForcingRotation = false,
    InstantRotationConnection = nil,
  }

  local function f93(p128, p129)
    local v177 = p129 - p128
    if v177 > 180 then v177 = v177 - 360 end
    if v177 < -180 then v177 = v177 + 360 end
    return v177
  end

  local function f94()
    local findFirstChild18
    if touchEnabled then
      findFirstChild18 = playerGui4:FindFirstChild("check", true)
      if findFirstChild18 and findFirstChild18:IsA("GuiObject") then
        local absolutePosition = findFirstChild18.AbsolutePosition
        local absoluteSize = findFirstChild18.AbsoluteSize
        local getGuiInset = guiService:GetGuiInset()
        local x = absolutePosition.X + absoluteSize.X / 2 + getGuiInset.X
        local y = absolutePosition.Y + absoluteSize.Y / 2 + getGuiInset.Y

        pcall(function()
          virtualInputManager:SendTouchEvent(8822, Enum.UserInputState.Begin.Value, x, y)
        end)
        task.wait(0.01)
        pcall(function()
          virtualInputManager:SendTouchEvent(8822, Enum.UserInputState.End.Value, x, y)
        end)
      end
    else
      pcall(function()
        virtualInputManager:SendKeyEvent(true, Enum.KeyCode.Space, false, game)
      end)
      task.wait(0.01)
      pcall(function()
        virtualInputManager:SendKeyEvent(false, Enum.KeyCode.Space, false, game)
      end)
    end
  end

  local function f95()
    for index36, value80 in ipairs({ "SkillCheckPromptGui", "SkillCheckPromptGui-con" }) do
      local findFirstChild19 = playerGui4:FindFirstChild(value80, true)
      if findFirstChild19 then
        local findFirstChild20 = findFirstChild19:FindFirstChild("Check", true)
        if findFirstChild20 and findFirstChild20.Visible then
          local findFirstChild21 = findFirstChild20:FindFirstChild("Line", true)
          local findFirstChild22 = findFirstChild20:FindFirstChild("Goal", true)
          if findFirstChild21 and findFirstChild22 then
            return findFirstChild21, findFirstChild22
          end
        end
      end
    end
  end

  local function f96()
    local v180, v181 = f95()
    if not (v180 and v181) then
      v176.InstantHasClicked = false
      v176.InstantLastGoalRotation = 0
      v176.InstantLastGoalInstance = nil
      v176.InstantCurrentGoalID = 0
      if v176.InstantRotationConnection then
        v176.InstantRotationConnection:Disconnect()
        v176.InstantRotationConnection = nil
      end
      return
    else
      local v182 = v181.Rotation % 360
      local rotation = (v182 + 106) % 360
      if not v176.InstantForcingRotation then
        v176.InstantForcingRotation = true
        pcall(function() v180.Rotation = rotation end)
        v176.InstantForcingRotation = false
      end
      local v183 = math.abs(v182 - v176.InstantLastGoalRotation)
      if v183 > 180 then v183 = 360 - v183 end
      if v183 > 0.5 or v176.InstantLastGoalInstance ~= v181 then
        v176.InstantHasClicked = false
        v176.InstantCurrentGoalID = v176.InstantCurrentGoalID + 1
        local instantCurrentGoalID = v176.InstantCurrentGoalID
        if v176.InstantRotationConnection then
          v176.InstantRotationConnection:Disconnect()
        end
        v176.InstantRotationConnection = v180:GetPropertyChangedSignal("Rotation"):Connect(function()
          if v176.InstantForcingRotation then return end
          v176.InstantForcingRotation = true
          pcall(function()
            local _, v185 = f95()
            if v185 then
              v180.Rotation = (v185.Rotation % 360 + 106) % 360
            end
          end)
          v176.InstantForcingRotation = false
        end)

        if not v176.InstantHasClicked then
          v176.InstantHasClicked = true
          task.spawn(function()
            task.wait(0.05)
            if v176.InstantCurrentGoalID == instantCurrentGoalID then
              local v186, v187 = f95()
              if v186 and v187 and tick() - v176.InstantLastTriggerTick > 0.03 then
                v176.InstantLastTriggerTick = tick()
                f94()
              end
            end
          end)
        end
      end
      v176.InstantLastGoalRotation = v182
      v176.InstantLastGoalInstance = v181
    end
  end

  local function f97(p130, p131, p132, p133)
    local function f100(p134)
      if p132 > p133 then
        return p134 >= p132 or p134 <= p133
      end
      return p134 >= p132 and p134 <= p133
    end
    if f100(p131) then return true end
    if p130 == nil then return false end
    local v202 = f93(p130, p131)
    local v203 = math.abs(math.floor(v202))
    if v203 < 2 then return false end
    local v204 = v202 / v203
    for i = 1, v203 do
      if f100((p130 + v204 * i) % 360) then return true end
    end
    return false
  end

  local function f98()
    local v188, v189 = f95()
    if not (v188 and v189) then
      v176.PerfectLastGoalRotation = nil
      v176.PerfectHasClickedThisGoal = false
      v176.PerfectLastLineRotation = nil
      v176.PerfectLastTick = nil
      v176.PerfectWasActive = false
      return
    end
    local v190 = v188.Rotation % 360
    local v191 = v189.Rotation % 360
    local v192 = os.clock()
    if not v176.PerfectWasActive then
      v176.PerfectWasActive = true
      v176.PerfectHasClickedThisGoal = false
      v176.PerfectLastGoalRotation = v191
      v176.PerfectLastLineRotation = v190
      v176.PerfectLastTick = v192
      return
    end
    if v176.PerfectLastGoalRotation and math.abs(f93(v176.PerfectLastGoalRotation, v191)) > 5 then
      v176.PerfectHasClickedThisGoal = false
      v176.PerfectLastLineRotation = nil
      v176.PerfectLastTick = nil
    end
    v176.PerfectLastGoalRotation = v191
    if v176.PerfectHasClickedThisGoal then
      v176.PerfectLastLineRotation = v190
      v176.PerfectLastTick = v192
      return
    end
    if v176.PerfectLastLineRotation and v176.PerfectLastTick then
      local v193 = v192 - v176.PerfectLastTick
      if v193 > 0 then
        local v194 = f93(v176.PerfectLastLineRotation, v190)
        if f97(v176.PerfectLastLineRotation, (v190 + v194 / v193 * v193 * 0) % 360, (v191 + 104) % 360, (v191 + 108) % 360) then
          v176.PerfectHasClickedThisGoal = true
          f94()
        end
      end
    end
    v176.PerfectLastLineRotation = v190
    v176.PerfectLastTick = v192
  end

  local function f99()
    local v195, v196 = f95()
    if not (v195 and v196) then
      v176.LastGoalRotation = nil
      v176.HasClickedThisGoal = false
      v176.LastLineRotation = nil
      v176.LastTick = nil
      v176.WasActive = false
      return
    end
    local v197 = v195.Rotation % 360
    local v198 = v196.Rotation % 360
    local v199 = os.clock()
    if not v176.WasActive then
      v176.WasActive = true
      v176.HasClickedThisGoal = false
      v176.LastGoalRotation = v198
      v176.LastLineRotation = v197
      v176.LastTick = v199
      return
    end
    if v176.LastGoalRotation and math.abs(f93(v176.LastGoalRotation, v198)) > 5 then
      v176.HasClickedThisGoal = false
      v176.LastLineRotation = nil
      v176.LastTick = nil
    end
    v176.LastGoalRotation = v198
    if v176.HasClickedThisGoal then
      v176.LastLineRotation = v197
      v176.LastTick = v199
      return
    end
    if v176.LastLineRotation and v176.LastTick then
      local v200 = v199 - v176.LastTick
      if v200 > 0 then
        local v201 = f93(v176.LastLineRotation, v197)
        if f97(v176.LastLineRotation, (v197 + v201 / v200 * v200 * 0) % 360, (v198 + 104) % 360, (v198 + 109) % 360) then
          v176.HasClickedThisGoal = true
          task.spawn(function()
            task.wait(0.03)
            f94()
          end)
        end
      end
    end
    v176.LastLineRotation = v197
    v176.LastTick = v199
  end

  runService.RenderStepped:Connect(function()
    if not VD.AutoSkillcheck then return end
    if VD.AutoSkillcheckMode == "Perfect" then
      f98()
    elseif VD.AutoSkillcheckMode == "Instant" then
      f96()
    else
      f99()
    end
  end)
end

f15()

if v31 then
  local survivorTab = v31:AddTab({ Name = "Survivor", Icon = "solar:shield-bold" })
  local generalSection = survivorTab:AddSection({ Name = "Skillcheck Features" })

  generalSection:AddToggle({
    Default = false,
    Name = "Auto Skillcheck",
    Flag = "Auto Skillcheck",
    Callback = function(state)
      VD.AutoSkillcheck = state == true
    end,
  })

  generalSection:AddDropdown({
    Name = "Skillcheck Mode",
    Flag = "Skillcheck Mode",
    Values = { "Normal", "Perfect", "Instant" },
    Default = "Normal",
    Callback = function(mode)
      if type(mode) == "table" then mode = mode[1] end
      VD.AutoSkillcheckMode = mode or "Normal"
    end,
  })
end

uiLib:Init()
