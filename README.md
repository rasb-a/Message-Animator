
## Table of Contents

-   [Summary](#Summary)
-   [Features](#Features)
-   [Installation](#Installation)
-   [Commands](#Commands)
-   [Configuration](#Configuration)
-   [Important Notes on Placeholders](#important-notes-on-placeholders)
-   [Suggestions & Feedback](#suggestions--feedback)

## Summary

Message Animator is a simple yet powerful plugin that allows you to display dynamic and customizable messages for your players. 
Compatible from 1.18 to 1.21.4
## Features


- **Custom Chat Messages**: Display personalized and animated messages in the chat for various events (e.g., player join, server announcements).  
- **Action Bar Messages**: Send engaging messages directly to the action bar.  
- **Boss Bar Animations**: Highlight players on login with fully customizable boss bars.  
- **Title & Subtitle**: Display dynamic titles and subtitles for player greetings or events.  
- **Song Playback**: Play unique sounds or music during player interactions (e.g., login).
- **Toast Display**: chose material, style and message
- **MiniMessage Support**: Use advanced formatting with [MiniMessage](https://docs.advntr.dev/minimessage/format.html) for rich text, gradients, colors, and more.

  
![Messsage Animator gif (3) (2)](https://github.com/user-attachments/assets/4ce71076-b367-439e-aede-eb6c90b81004)



## Installation

1. Download the plugin jar file in [Spigot]() ,[Builtbybit]() or [Polymart]() .
2. Place it in your server's "plugins" folder.
3. Restart your server.
4. You're ready to go! **Message Animator** works out of the box with default settings.  

## Commands

| **Command**        | **Description**                 | **Permission**              |
|---------------------|---------------------------------|-----------------------------|
| `/ma reload`       | Reloads the plugin's settings. | `messageAnimator.reload`    |
| `/ma preview <all ><title> <message> <bossbar> <actionbar> <toast> <sound> `       | Preview the plugin's settings. | `messageAnimator.preview`    |

---
## Configuration

Below is the default configuration file for **Message Animator**. Customize it to fit your server's style!


```yaml
# !-----------------------------------------------------------------------------------------------!
#                       Welcome to the main configuration of MessageAnimator
# !-----------------------------------------------------------------------------------------------!

#COLOR CODES are supported with the '&' character.
#       - For usage, see https://minecraft.tools/fr/color-code.php or https://docs.advntr.dev/minimessage/format.html
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
```

## Important Notes on Placeholders

Important Notes on Placeholders
Supported placeholders:
The plugin fully supports placeholders such as %luckperms_prefix%, %player_name%, and more.

Hex color limitations:
Placeholders containing HEX colors in the &# format (e.g., &#FF5733) are NOT SUPPORTED.
To use HEX colors, replace the &# prefix with #. For example:

```yaml

Correct: <#FF5733>This is supported</#FF5733>  
Incorrect: <&#FF5733>This will not work</&#FF5733>
```
For advanced placeholders and color customization, visit the [MiniMessage documentation](https://docs.advntr.dev/minimessage/format.html).


Example for %luckperms_prefix% with HEX colors 

```yaml
Modifier
Message: '<#FF5733>%luckperms_prefix% <#FFFFFF>Welcome, %player_name%!</#FFFFFF>'
```

## Suggestions & Feedback
If you have any suggestions, feedback, or feature requests, feel free to open an issue on our GitHub page. We appreciate your input to make **Message Animator** even better!




