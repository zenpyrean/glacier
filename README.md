# SECTION 1: EXECUTION & SYNTAX GUIDE

## Overview

Glacier is heavily inspired by *Adonis Admin*, sharing many similarities in command execution and structure. The primary method for executing commands is through the **command bar**, which is triggered by pressing **Right Shift**. Unlike some other admin systems, commands in Glacier **do not require a prefix**.

---

## Player Selectors

Commands that accept players as arguments support either:

* A **single player**
* A **comma-separated list of player names**

**Example:**

```text
kill player
kill player1,player2
```

**Notes:**

* Player names are **case-insensitive** and accept **partial matches**.
* If multiple players match a partial name, the command will **not execute**.

---

### Special Identifiers

Glacier supports special selectors for targeting specific groups of players:

| Selector     | Description                                                          |
| ------------ | -------------------------------------------------------------------- |
| `me`         | The executor of the command                                          |
| `all`        | All players in the server                                            |
| `others`     | Everyone except the executor                                         |
| `admins`     | All admins (rank `moderator` or higher)                              |
| `nonadmins`  | Everyone except admins (rank `moderator` or higher)                  |
| `#NUM`       | Randomly selects a specified number of players                       |
| `@USERNAME`  | Targets a player whose username matches exactly (case-insensitive)   |
| `%TEAM`      | Targets all players on a specified team                              |
| `radius-NUM` | Targets players within a specific radius (in studs) — *TO IMPLEMENT* |

**Inversion:**
Prepending `-` to a selector inverts the selection.
**Example:**

```text
kill -radius-10
```

Kills all players further than 10 studs away from the executor — *TO IMPLEMENT*

---

## Batch & Delayed Commands

Glacier supports executing multiple commands sequentially or with delays:

* **Sequential execution:** Use `//` to separate commands.
* **Delayed execution:** Use `wait NUM` to delay subsequent commands by `NUM` seconds.

**Example:**

```text
m Everyone will die in 10 seconds! // wait 10 // kill all
```

This example:

1. Sends a message announcement
2. Waits 10 seconds
3. Kills all players
   (*TO IMPLEMENT*)

---

# SECTION 2: COMMAND USAGE

*Content pending or can be filled with a list of available commands and syntax examples.*

---

# SECTION 3: CUSTOM COMMANDS

## Creating Custom Commands

Glacier provides a straightforward method for defining custom commands. *Details on usage, syntax, and examples can be provided here.*
