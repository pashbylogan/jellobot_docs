# Discord Commands

## Table of Contents

- [on_ready](#on_ready)
- [ping](#ping)
- [send_times_msg](#send_times_msg)
- [on_message_delete](#on_message_delete)
- [clearall](#clearall)
- [eg](#eg)
- [transfer](#transfer)
- [monthtransfer](#monthtransfer)
- [close](#close)
- [r](#r)
- [add main](#addmain)
- [add alt](#addalt)
- [add class](#addclass)
- [add nickname](#addnick)
- [abbreviations](#abbrev)
- [chars](#chars)
- [loot](#loot)
- [bids](#bids)
- [top](#top)
- [points](#points)

### on_ready`#!py3 ()` { #on_ready data-toc-label=on_ready }

This function is executed when the bot is ready.

### ping`#!py3 (ctx: commands.Context)` { #ping data-toc-label=ping }

Send a "Pong!" message to the given context.

Parameters

> ctx: `commands.Context` -- Description of parameter `ctx`.

### send_times_msg`#!py3 (message: discord.Message)` { #send_times_msg data-toc-label=send_times_msg }

Record attendance upon receiving a message in a specific channel.

Parameters

> message: `discord.Message` -- Description of parameter `message`.

### on_message_delete`#!py3 (message: discord.Message)` { #on_message_delete data-toc-label=on_message_delete }

Remove attendance when a message is deleted in a specific channel.

Parameters

> message: `discord.Message` -- Description of parameter `message`.

??? warning "warning block"
    Discord keeps a cache of recent messages that are kept for some unknown amount of time. on_message_delete depends on that cache: if the message is no longer cached it can't receive the message content and this function breaks.

### clearall`#!py3 (ctx: commands.Context)` { #clearall data-toc-label=clearall }

Clear all boss timers. Admins only.

Parameters

> ctx: `commands.Context` -- Description of parameter `ctx`.

### eg`#!py3 (ctx: commands.Context)` { #eg data-toc-label=eg }

Record elite guard attendance.

Parameters

> ctx: `commands.Context` -- Description of parameter `ctx`.

### transfer`#!py3 (ctx: commands.Context)` { #transfer data-toc-label=transfer }

Transfer attendance between players.

Parameters

> ctx: `commands.Context` -- Description of parameter `ctx`.

### monthtransfer`#!py3 (ctx: commands.Context)` { #monthtransfer data-toc-label=monthtransfer }

Transfer KP between players on a monthly basis.

Parameters

> ctx: `commands.Context` -- Description of parameter `ctx`.

### close`#!py3 (ctx: commands.Context)` { #close data-toc-label=close }

Close bids for an item and assign it to the winning player.

Parameters

> ctx: `commands.Context` -- Description of parameter `ctx`.

### r`#!py3 (ctx: commands.Context)` { #r data-toc-label=r }

Return an item and refund the KP.

Parameters

> ctx: `commands.Context` -- Description of parameter `ctx`.

### Add Main Player `#!py3 (ctx: commands.Context, player_name: str, nickname: str)` { #addmain }

Add a main player with their initial nickname.

Parameters

> ctx: `commands.Context` -- The context in which the command was called.

> player_name: `str` -- Name of the main player to be added.

> nickname: `str` -- Initial nickname of the main player.

---

### Add Alternate Character `#!py3 (ctx: commands.Context, main_nickname: str, alt_player_name: str, nickname: str)` { #addalt }

Add an alternate character to the main player with their initial nickname.

Parameters

> ctx: `commands.Context` -- The context in which the command was called.

> main_nickname: `str` -- Nickname of the main player the alternate character will be linked to.

> alt_player_name: `str` -- Name of the alternate character to be added.

> nickname: `str` -- Initial nickname of the alternate character.

---

### Add Nickname `#!py3 (ctx: commands.Context, player_nickname: str, new_nickname: str)` { #addnick }

Add a new nickname to an existing player.

Parameters

> ctx: `commands.Context` -- The context in which the command was called.

> player_nickname: `str` -- Existing nickname of the player.

> new_nickname: `str` -- New nickname to be added to the player.

---

### Add Class `#!py3 (ctx: commands.Context, player_nickname: str, class_name: str)` { #addclass }

Add a class to an existing player.

Parameters

> ctx: `commands.Context` -- The context in which the command was called.

> player_nickname: `str` -- Existing nickname of the player.

> class_name: `str` -- Class to be added to the player. Valid classes are 'rogue', 'warrior', 'lock rogue', 'mage', 'druid', and 'ranger'.

### Abbreviations `#!py3 (ctx: commands.Context)` { #abbrev }

Send a list of abbreviations used in the system.

Parameters

> ctx: `commands.Context` -- The context in which the command was called.

---

### Chars `#!py3 (ctx: commands.Context)` { #chars }

Get the characters associated with a main player by their name or nickname.

Parameters

> ctx: `commands.Context` -- The context in which the command was called.

---

### Loot `#!py3 (ctx: commands.Context)` { #loot }

Get the loot history of a player by their name or nickname.

Parameters

> ctx: `commands.Context` -- The context in which the command was called.

---

### Bids `#!py3 (ctx: commands.Context)` { #bids }

Get the bid history of an item by its name.

Parameters

> ctx: `commands.Context` -- The context in which the command was called.

---

### Top `#!py3 (ctx: commands.Context)` { #top }

Get the top players by a specified ranking type, with optional class filtering.

Parameters

> ctx: `commands.Context` -- The context in which the command was called.

---

### Points `#!py3 (ctx: commands.Context)` { #points }

Get the points and monthly attendance of a player by their name or nickname.

Parameters

> ctx: `commands.Context` -- The context in which the command was called.
