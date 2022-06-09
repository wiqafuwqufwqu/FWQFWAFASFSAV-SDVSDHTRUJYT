local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local whitelistUserIDs = {}

game.Players.PlayedAdded:Connect(function(player)
    if not table.find(whitelistUserIDs,player.UserId) then --If the UserID value is not in the table this returns nil. In Lua nil equals false.
        player:Kick("You are not whitelisted on this server.")
            end
end)
local Window = Library.CreateLib("TITLE", "DarkTheme")
local Tab = Window:NewTab("TabName")
local Section = Tab:NewSection("Section Name")
