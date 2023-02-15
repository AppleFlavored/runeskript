# RuneSkript
A scripting language that compiles into [Skript](https://github.com/SkriptLang/Skript).

## Example Syntax
This example was converted from the [Skript documentation](https://docs.skriptlang.org/).

```
on player join:
    format = "%player%: %message%"

command /sethome:
    if {home::%uuid of player%} is not set:
        player.send("You have not set your home yet!")
        stop
    
    player.teleport({home::%uuid of player%})
    player.send("&aYou have been teleported.")
```

## License
RuneSkript is licensed under the MIT License. See [LICENSE](LICENSE) for more details.