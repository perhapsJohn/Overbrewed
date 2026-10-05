# Overbrewed (web build)

Co-op Halloween potion brewing for 1-4 monsters: chop newt eyes, grind bat
wings, keep the cauldrons from boiling over and get the potions out of the
hatch before the moon sets. Solo with bot helpers, couch co-op, or online rooms
through the Wayside relay. Made in Godot 4.6; this is the browser build, also
a cart in the Wayside Station arcade.

One page, two packs: phones and tablets load `index.mobile.pck` (lighter
graphics, fewer music tracks), desktop browsers `index.pck`.
`?pack=mobile|desktop` forces one; `?room=CODE` opens a friend's online room.
At the end of an Endless Night run the game posts
`{type: "PLAYER_DIED", score}` (the crew's coins) to the page around it.

This repo holds only the exported files; the game's source lives elsewhere
and publishes here with its `tools/publish_web.sh`.
