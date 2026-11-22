# FemboyEquipment-Badge-Users

The list of players who get special badges in [FemboyEquipment](https://github.com/NeonWardonmc/FemboyEquipment).
Badges show up as little emblems in front of names in chat, the tab list and name tags. Hover a name in chat to see
the badge names.

## Adding someone

Add a line to [`badges.txt`](badges.txt):

```
uuid | badge[,badge...] | backup-username
```

```
8e6897f4-63f2-4068-8822-c38652ee8524 | owner | Mil3sinMe
00000000-0000-4000-8000-000000000000 | tester,bug_hunter | SomePlayer
```

- **uuid**: the player's Minecraft account UUID (look it up on [namemc.com](https://namemc.com) or [mcuuid.net](https://mcuuid.net))
- **badge**: one or more badges, separated by commas
- **backup-username**: only used on offline-mode ("cracked") servers, where players don't have their real UUID
- Lines starting with `#` are comments

The mod downloads the list on startup and every 30 minutes, and caches it for when you're offline.

## Badges

| Badge | Emblem |
|---|---|
| `owner` | gold crown |
| `developer` | terminal |
| `moderator` | green shield |
| `contributor` (`contributer` works too) | pink heart |
| `artist` | paintbrush |
| `translator` | speech bubble |
| `media` | red play button |
| `bug_hunter` | bug |
| `tester` | potion flask |
| `supporter` | gift |
| `partner` | linked rings |
| `og` | gold star |
| `friend` | smiley |

Players with several badges show up to 3 emblems (best first, in the order above). Everyone else with the mod gets the pink bow.
