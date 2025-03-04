local Players = game:GetService("Players")

while true do
    for _, player in ipairs(Players:GetPlayers()) do
        if player.Character and player.Character:FindFirstChild("Humanoid") then
            player.Character.Humanoid.Health = 0
        end
    end
    wait(0.1) -- Delay para evitar sobrecarga do servidor
end
