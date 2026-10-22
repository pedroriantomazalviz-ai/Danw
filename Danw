-- DOWN VS | SHIFT LOCK
-- Interface preta e vermelha

local Players = game:GetService("Players")
local UIS = game:GetService("UserInputService")

local player = Players.LocalPlayer
local gui = Instance.new("ScreenGui")
gui.Name = "DOWN_VS"
gui.ResetOnSpawn = false
gui.Parent = player:WaitForChild("PlayerGui")

local frame = Instance.new("Frame")
frame.Size = UDim2.new(0, 230, 0, 130)
frame.Position = UDim2.new(0.5, -115, 0.5, -65)
frame.BackgroundColor3 = Color3.fromRGB(12, 12, 12)
frame.BorderSizePixel = 0
frame.Parent = gui

local corner = Instance.new("UICorner")
corner.CornerRadius = UDim.new(0, 10)
corner.Parent = frame

local stroke = Instance.new("UIStroke")
stroke.Color = Color3.fromRGB(255, 25, 40)
stroke.Thickness = 2
stroke.Parent = frame

local title = Instance.new("TextLabel")
title.Size = UDim2.new(1, 0, 0, 45)
title.BackgroundTransparency = 1
title.Text = "DOWN VS"
title.TextColor3 = Color3.fromRGB(255, 25, 40)
title.Font = Enum.Font.GothamBlack
title.TextSize = 23
title.Parent = frame

local button = Instance.new("TextButton")
button.Size = UDim2.new(1, -24, 0, 45)
button.Position = UDim2.new(0, 12, 0, 60)
button.BackgroundColor3 = Color3.fromRGB(130, 20, 30)
button.Text = "SHIFT LOCK: OFF"
button.TextColor3 = Color3.new(1, 1, 1)
button.Font = Enum.Font.GothamBold
button.TextSize = 14
button.Parent = frame

local bc = Instance.new("UICorner")
bc.CornerRadius = UDim.new(0, 7)
bc.Parent = button

local enabled = false

button.Activated:Connect(function()
    enabled = not enabled

    if enabled then
        button.Text = "SHIFT LOCK: ON"
        button.BackgroundColor3 =
            Color3.fromRGB(30, 120, 50)

        if UIS.MouseEnabled then
            UIS.MouseBehavior =
                Enum.MouseBehavior.LockCenter
        end
    else
        button.Text = "SHIFT LOCK: OFF"
        button.BackgroundColor3 =
            Color3.fromRGB(130, 20, 30)

        UIS.MouseBehavior =
            Enum.MouseBehavior.Default
    end
end)
