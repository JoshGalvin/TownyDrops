TownyDrops Minecraft Plugin
------------------------------
v.1.0.0

This requires Towny to use but enables use to set drop rates/amount/bonus of blocks by town. This is useful for making
Mining towns vs Lumber Towns vs your Imagination.

commands:

    droprate:
        description: You can adjust the drop rate of materials in the world.
        permission: wog.droprate
        usage: |
            /<command> [TYPE] [PERCENTAGE] |
            /<command> [TOWN] [TYPE] [PERCENTAGE CHANCE]
    dropamount:
        description: You can adjust the drop amount of materials for a specific town and chance.
        permission: wog.dropamount
        usage: |
            /<command> [TOWN] [TYPE] [ADDITIONAL AMOUNT] [PERCENTAGE CHANCE]
    dropchance:
        description: You can add a % chance to drop another item from a completely different block!
        permission: wog.dropchance
        usage: |
            /<command> [TOWN] [TYPE] [TYPE] [ADDITIONAL AMOUNT] [PERCENTAGE CHANCE]
    droprates:
        description: List the current drop rates of materials.
        permission: wog.droprates
        usage: |
            /<command>
    dropamounts:
        description: List the drop amounts for a specific player.
        permission: wog.dropamounts
        usage: |
            /<command> [PLAYER]
permissions:

    wog.*:
        description: Full access to the World of Gods commands
        children:
            wog.droprate: true
            wog.dropamount: true
            wog.droprates: true
            wog.dropamounts: true
            wog.dropchance: true
    wog.droprate:
        description: Allows users to adjust the drop rate of materials in the world.
        default: false
    wog.dropamount:
        description: Allows users to adjust the drop rate of materials in the world.
        default: false
    wog.droprates:
        default: false
    wog.dropamounts:
        default: false
    wog.dropchance:
        default: false