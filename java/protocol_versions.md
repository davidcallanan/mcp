# Protocol Versions

Protocol versions numbers are used to determine compatibility between a client and server for a specific version of the game.

You can find a list of protocol numbers and their corresponding Minecraft versions [on the Minecraft wiki here](https://minecraft.gamepedia.com/Java_Edition_data_value/Protocol_and_data_versions).

## Universal Protocol Version Number (UPVN)

This project uses a 4-digit hexadecimal protocol version format which can also distinguish between Pre-Netty and Post-Netty versions. This version number may be prefixed with a `j` character to denote the Java Edition of Minecraft.

The UPVN can be obtained by performing the appropriate calculation as follows and then converting the result to a 4-digit HEX number (and optionally prefixing it with a `j`):

 - For Pre-Netty versions, the UPVN is equal to the Protocol Number.
 - For Post-Netty versions, `0x51` must be added to the Protocol Number to obtain the UPVN.

