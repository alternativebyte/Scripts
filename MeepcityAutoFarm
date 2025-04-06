local connection=game.ReplicatedStorage.Connection
local vw=workspace.VW
connection:InvokeServer(9, 1)
game:GetService("RunService").RenderStepped:Connect(function()
    connection:InvokeServer(49)
    connection:InvokeServer(50)
    connection:InvokeServer(51)
    local fish = vw:FindFirstChild("TempFish")
    if fish then
        local fishData = {
            ["FishingPolePos"] = fish.Position,
            ["Power"] = 1,
            ["Face"] = fish.Position,
            ["PlayerPos"] = fish.Position,
            ["FishingZonePos"] = Vector3.new(-5.29345703, -18.0412292, 43.7173767)
        }
        connection:InvokeServer(11, fishData)
    end
end)  
