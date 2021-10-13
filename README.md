Version 2.0 by MonkeyWhisper#0001

# Added qb-target support

Download from here : https://github.com/BerkieBb/qb-target

# Add to Config.BoxZones

        ["jewelheist"] = {
        name = "jewelheist",
        coords = vector3(-595.8919, -283.6023, 50.3237),
        length = 1.00,
        width = 1.00,
        heading = 302.7994,
        debugPoly = true,
        minZ = 50.00,
        maxZ = 51.40,
        options = {
            {
              type = "client",
              event = "qb-jewellery:client:startheist",
              icon = "fas fa-video",
              label = "Disable Cameras",
            },
        },
        distance = 5.0
    },
    
    ["jewelheistdoor"] = {
        name = "jewelheistdoor",
        coords = vector3(-619.9963, -223.90, 38.3175),
        length = 0.30,
        width = 0.40,
        heading = 38.5005,
        debugPoly = false,
        minZ = 38.50,
        maxZ = 38.80,
        options = {
            {
              type = "client",
              event = "qb-jewellery:client:UsePinkCard",
              icon = "fas fa-id-card-alt",
              label = "Disable Doors",
            },
        },
        distance = 5.0
    },

# Add to Config.TargetModels

    ["jewelboxes"] = {
        models = {
            `des_jewel_cab3_start`,
            `des_jewel_cab2_start`,
            `des_jewel_cab_start`,
            `des_jewel_cab4_start`,

        },
        options = {
            {
                type = "client",
                event = "qb-jewellery:client:startbreakinglass",
                icon = "fas fa-gem",
                label = "Break Glass",
            },
        },
        distance = 4.0
    },

# Preview:

https://imgur.com/gkzpoB2

Version 1.0 by Lion Heart

# Jewellery Store Robbery Reworked
Reworked jewellery store robbery for qbus base. Players now have to hack the security system on the roof to gain access to the store.
After 90 seconds the store goes into lockdown and the front door is locked again. Without a security card the robbers are trapped inside.

# FAQ:
Q: My door is not unlocking
A: Change the doorId in 'TriggerServerEvent('qb-doorlock:server:updateState', 137, false/true)' to your corresponding qb-doorlock doorId

# Dependency: 
mobile hacking (https://github.com/GHMatti/FiveM-Scripts/tree/master/mhacking)

# Preview: 
https://streamable.com/go6ls2

# Support
If you need support, contact me on discord: Lionh34rt#7553

Follow me on twitch: https://twitch.tv/lionh34rtcs
