# Better-Mouseover-Tooltip
World of Warcraft addon that anchors in-game tooltip to the mouse with a pleasant offset!

Since Blizzard won't allow us to control how the tooltip is anchored and with which offset, I created this simple addon that does it for them!

This addon doesn't use the tooltip:SetOwner(parent, "ANCHOR_CURSOR") function, at least not just it. At the time of writing, this function doesn't allow for any kind of offset to it, which looks stupid. Downside is - the addon uses OnUpdate, which comes with a small cost to CPU usage. While stress testing on my 4060, it used at most 0.1% of CPU. If that's a lot or not is up to you.

If you want to change the offset, just head over to the addon's lua file, open it with Notepad, and adjust the values applied to xValue and yValue variables (1 and 11 by default).
