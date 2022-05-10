# ROBLOX GRAB AVATAR
## For avatar designers, by an avatar designer who happens to have coding experience
### by gamer0kayf1n3

1. Open Roblox Studio. https://www.roblox.com/create
2. Create a new project, and publish it, just dont make it public. This is important for requests to work.
3. ServerScriptService > Script
4. **create a Server Script in ServerScriptService, and paste any of the versions available, unobfuscated, obfuscated 1, obfuscated 2.**
5. Run server, go to server side, select the Humanoid, and File > Export to OBJ.
6. Get Blender, if you don't yet. https://blender.org/download
7. Import OBJ to Blender, and enable Cycles renderer.
8. Pose it to your liking, and do your usual designing workflow.

**note, replace ID value with either Discord ID or Roblox ID. If you have their Roblox username, use that instead, this script uses the BloxLink API, a popular discord Bot**

**create a Server Script in ServerScriptService, and paste any of the versions available, unobfuscated, obfuscated 1, obfuscated 2.**

Testing values:
Discord ID: 695104034297610290
Roblox ID: 1311038672
Username: 0kayf1n3

Test any of the values put above, and replace it in the variables



```lua
-- version, unobfuscated

-- init
local Players = game:GetService("Players")
local webapi = game:GetService("HttpService")

-- inputs
-- leave uname as nil if you have Discord ID or Roblox ID
local ID = "REPLACE ID WITH ROBLOX/DISCORD ID"
local uname = nil

-- determining data types
if uname ~= nil then
	print('this is a username')
	pcall(function () 
		rbid = Players:GetUserIdFromNameAsync(uname) 
	end)
elseif #ID >= 17 then
	print('this is a discord ID')
	bloxapi = webapi:JSONDecode(
		webapi:GetAsync("https://api.blox.link/v1/user/"..ID)
	)
	if bloxapi.status == "ok" then
		rbid = bloxapi.primaryAccount
	else
		print('fail')
	end
else
	print('this is a Roblox ID')
	rbid = ID
end
print(rbid)
function player_is_added(player)
	player.CharacterAppearanceId = rbid
	player:LoadCharacter()
end

for _, player in pairs (Players:GetPlayers()) do
	player_is_added(player)
end

Players.PlayerAdded:Connect(player_is_added)
```



```lua
-- version, obfuscated, level 1
local ajajajajaajajajaja = "868072467992809513" -- PLACE DISCORD/ROBLOX ID HERE
local aajajajaja = nil -- PLACE USERNAME HERE IF DISCORD/ROBLOX ID NOT AVAILABLE
ajajajajaaaajajajaja=game local ajajajajaajajajajaaa=ajajajajaaaajajajaja:GetService("Players")local ajajajajaajajajaj=ajajajajaaaajajajaja:GetService("HttpService")if aajajajaja~=nil then print('this is a username') pcall(function ()  ajajajajaajajajajajajajajaajajajajid=ajajajajaajajajajaaa:GetUserIdFromNameAsync(aajajajaja) end)elseif #ajajajajaajajajaja>=17 then print('this is a discord ID')ajajajajaajajajajajajajajaajajajaj=ajajajajaajajajaj:JSONDecode( ajajajajaajajajaj:GetAsync("https://api.blox.link/v1/user/"..ajajajajaajajajaja))if ajajajajaajajajajajajajajaajajajaj.status=="ok" then ajajajajaajajajajajajajajaajajajajid=ajajajajaajajajajajajajajaajajajaj.primaryAccount else print('fail')end else print('this is a Roblox ID') ajajajajaajajajajajajajajaajajajajid=ajajajajaajajajaja end print(ajajajajaajajajajajajajajaajajajajid)function ajajajajaajajajajajajajajaajajajajplaad(ajajajajaajajajajajajajajaajajajajpla)ajajajajaajajajajajajajajaajajajajpla.CharacterAppearanceId=ajajajajaajajajajajajajajaajajajajid ajajajajaajajajajajajajajaajajajajpla:LoadCharacter()end for ajajajjadasd, ajajajajaajajajajajajajajaajajajajpla in pairs (ajajajajaajajajajaaa:GetPlayers()) do ajajajajaajajajajajajajajaajajajajplaad(ajajajajaajajajajajajajajaajajajajpla)end ajajajajaajajajajaaa.PlayerAdded:Connect(ajajajajaajajajajajajajajaajajajajplaad)
```
```lua
-- version, obfuscated level 2

local JC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2c = "REPLACE DISCORD ID OR ROBLOX ID"
local uname = nil
function yvfU8xK_VQ6yvfU8xK_VQ6yvfU8xK_VQ6yvfU8xK_VQ6yvfU8xK_VQ (yvfU8xK_VQ) print(yvfU8xK_VQ) end FDG1AUN53S8FDG1AUN53S8FDG1AUN53S8FDG1AUN53S8FDG1AUN53S8 = game function N8nGig78lNs(N8nGig78lNs) return string.char(N8nGig78lNs) end local dQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQ = FDG1AUN53S8FDG1AUN53S8FDG1AUN53S8FDG1AUN53S8FDG1AUN53S8:GetService("Players")local Hh2e9_bGSysHh2e9_bGSysHh2e9_bGSysHh2e9_bGSysHh2e9_bGSys = FDG1AUN53S8FDG1AUN53S8FDG1AUN53S8FDG1AUN53S8FDG1AUN53S8:GetService("HttpService") if uname ~= nil then print(N8nGig78lNs(116)..N8nGig78lNs(104)..N8nGig78lNs(105)..N8nGig78lNs(115)..N8nGig78lNs(32)..N8nGig78lNs(105)..N8nGig78lNs(115)..N8nGig78lNs(32)..N8nGig78lNs(97)..N8nGig78lNs(32)..N8nGig78lNs(117)..N8nGig78lNs(115)..N8nGig78lNs(101)..N8nGig78lNs(114)..N8nGig78lNs(110)..N8nGig78lNs(97)..N8nGig78lNs(109)..N8nGig78lNs(101)) pcall(function () al1BNB8bKaEal1BNB8bKaEal1BNB8bKaEal1BNB8bKaEal1BNB8bKaE = dQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQ:GetUserIdFromNameAsync(uname) end) elseif #JC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2c >= 17 then print(N8nGig78lNs(116)..N8nGig78lNs(104)..N8nGig78lNs(105)..N8nGig78lNs(115)..N8nGig78lNs(32)..N8nGig78lNs(105)..N8nGig78lNs(115)..N8nGig78lNs(32)..N8nGig78lNs(97)..N8nGig78lNs(32)..N8nGig78lNs(100)..N8nGig78lNs(105)..N8nGig78lNs(115)..N8nGig78lNs(99)..N8nGig78lNs(111)..N8nGig78lNs(114)..N8nGig78lNs(100)..N8nGig78lNs(32)..N8nGig78lNs(73)..N8nGig78lNs(68)) bloxapi = Hh2e9_bGSysHh2e9_bGSysHh2e9_bGSysHh2e9_bGSysHh2e9_bGSys:JSONDecode( Hh2e9_bGSysHh2e9_bGSysHh2e9_bGSysHh2e9_bGSysHh2e9_bGSys:GetAsync("https://api.blox.link/v1/user/"..JC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2c)) if bloxapi.status == "ok" then al1BNB8bKaEal1BNB8bKaEal1BNB8bKaEal1BNB8bKaEal1BNB8bKaE = bloxapi.primaryAccount else print(N8nGig78lNs(102)..N8nGig78lNs(97)..N8nGig78lNs(105)..N8nGig78lNs(108))end else print(N8nGig78lNs(116)..N8nGig78lNs(104)..N8nGig78lNs(105)..N8nGig78lNs(115)..N8nGig78lNs(32)..N8nGig78lNs(105)..N8nGig78lNs(115)..N8nGig78lNs(32)..N8nGig78lNs(97)..N8nGig78lNs(32)..N8nGig78lNs(82)..N8nGig78lNs(111)..N8nGig78lNs(98)..N8nGig78lNs(108)..N8nGig78lNs(111)..N8nGig78lNs(120)..N8nGig78lNs(32)..N8nGig78lNs(73)..N8nGig78lNs(68)) al1BNB8bKaEal1BNB8bKaEal1BNB8bKaEal1BNB8bKaEal1BNB8bKaE = JC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2cJC0mFHN7r2c end print(al1BNB8bKaEal1BNB8bKaEal1BNB8bKaEal1BNB8bKaEal1BNB8bKaE) function T59N3DPrvacT59N3DPrvacT59N3DPrvacT59N3DPrvacT59N3DPrvac(yPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmA) yPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmA.CharacterAppearanceId = al1BNB8bKaEal1BNB8bKaEal1BNB8bKaEal1BNB8bKaEal1BNB8bKaE yPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmA:LoadCharacter() end for _, yPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmA in pairs (dQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQ:GetPlayers()) do T59N3DPrvacT59N3DPrvacT59N3DPrvacT59N3DPrvacT59N3DPrvac(yPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmAyPYZpwSpKmA)end dQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQdQw4w9WgXcQ.PlayerAdded:Connect(T59N3DPrvacT59N3DPrvacT59N3DPrvacT59N3DPrvacT59N3DPrvac)
```
