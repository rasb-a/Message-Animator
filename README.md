
## Table of Contents

-   [Summary](#Summary)
-   [Features](#Features)
-   [Installation](#Installation)
-   [Commands](#Commands)
-   [Configuration](#Configuration)

## Summary

Message Animator is a simple yet powerful plugin that allows you to display dynamic and customizable messages for your players. 
Compatible from 1.18 to 1.21.4
## Features

Custom Chat Messages: Display personalized messages in the chat for various events (e.g., player join, announcements).
Action Bar Messages: Show messages in the action bar for additional player engagement.
Boss Bar: Highlight players on login with customizable boss bar messages.
Title & Subtitle: Display animated titles and subtitles to welcome players or show server events.
Song Playback: Play custom music when players log in to create a unique experience.
MiniMessage Support: Easily format messages using MiniMessage from Guardian, with support for rich text, colors, and styles.

## Installation

1. Download the plugin jar file in [Spigot]() ,[Builtbybit]() or [Polymart]() .
2. Place it in your server's "plugins" folder.
3. Restart your server.
4. Ho no four
No further configuration needed! **Message Animator** will work out of the box

## Commands

/ma reload for the reload a plugin 
permission : messageAnimator.reload

## Configuration
```yaml
# !-----------------------------------------------------------------------------------------------!
#                       Welcome to the main configuration of MessageAnimator
# !-----------------------------------------------------------------------------------------------!

#COLOR CODES are supported with the '&' character.
#       - For usage, see http://minecraftwiki.net/wiki/Formatting_codes or https://docs.advntr.dev/minimessage/format.html
#       - For  message viewver https://www.birdflop.com/resources/rgb/ or https://webui.advntr.dev/
# -------------------------------------------------------------------------------------------------

#Title Message
TitleEnable: true
Title: <gradient:#FE5C2A:#CF1F2B>Welecom to (you<gradient:#CF1F2B:#F2C6DE>r serveur name)</gradient>
SubTitle: <gradient:#CF1F2B:#F2C6DE>Enjoy your stay </gradient><gradient:#F2C6DE:#FE5C2A>, %player_name%</gradient>
FadeIn: 2
FadeOut: 3
Stay: 2

#Message
MessageEnable: true
Message:
- '<gradient:#4DECC9:#E03292>Hello %player_name%, w</gradient><gradient:#E03292:#FE5C2A>elcome to our server!</gradient>'
- '<gradient:#E03292:#4DECC9>We hope you have </gradient><gradient:#4DECC9:#FE5C2A>an amazing time!</gradient>'
- '<gradient:#FE5C2A:#4DECC9>Explore, build, and ha</gradient><gradient:#4DECC9:#E03292>ve <hover:show_text:''this fun''>fun</hover>  %player_name%</gradient>'
- '<gradient:#FE5C2A:#4DECC9>Need help? </gradient><gradient:#4DECC9:#E03292><click:run_command:''/help''>Click here!</click></gradient>'

#Boss Bar for the format :progress, notched_6, notched_10, notched_12, notched_20
BossBarEnable: true
BossBarMessage: <rainbow>Welcome %player_name% to the adventure!<rainbow>
BossBarDelay: 6
BossBarColor: PINK
BossBarFormat: notched_6

#ActionBar
ActionBarEnable: true
ActionTitle: <gradient:#FE5C2A:#F2C6DE>re playing as </gradient><gradient:#F2C6DE:#CF1F2B>%player_name%! Have fun!</gradient>

#Sound  please check list https://hub.spigotmc.org/javadocs/bukkit/org/bukkit/Sound.html
SoundEnable: true
Sound: BLOCK_AMETHYST_BLOCK_HIT



