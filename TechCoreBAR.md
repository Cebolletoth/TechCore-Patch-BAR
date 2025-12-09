# TechCore-Patch-BAR
Hosting site for the updated information and tweakcodes of the BAR TechCore initiative.

------

# README - TECH CORE PATCH
 
Made by C3BO in the spirit of MeowCatMeow’s economic system overhaul.
Feedback to BAR Discord thread
https://discord.com/channels/549281623154229250/1447223310319489024

TechCores rely on the infrastructure provided by Seth's TechBlocking modoption which he kindly allowed us to use for this public initiative.
- This requires the use of a tweakdef (code provided) to supress the original passive lab xp generation from the modoption.
- The use of extra experimental game assets requires enabling the *"Force Load All Units"* tickbox under the Advanced lobby options - Cheat section.

The Techcore patch tweakunits restricts the player/team's ability to build higher tech level factories by requiring them to "research" the technology first. Each TechCore building (experimental armada airlab available to all T1cons buildmenu) provides a single TechPoint that counts towards permanently unlocking the next tier level as long as the building is alive. Losing unlocked tech tiers is not possible despite losing techcores after that point.
- The research thresholds can be set by using the control panel of the Techblocking modoption.
- Recommended initial testing parameters: Set to **points per team (by unticking the per player box), 50% (roundedup) of TeamSize for T2 and 100% of Team Size for T3.
```
Team size - T2 - T3
1         - 1  - 1
2         - 1  - 2
3         - 2  - 3
4         - 2  - 4
5         - 3  - 5
6         - 3  - 6
7         - 4  - 7
8         - 4  - 8
```
-----
# Lobby settings photo reference (8v8 limits)
<img width="743" height="566" alt="image" src="https://github.com/user-attachments/assets/0632244e-d400-4f4b-a28e-ee539302615c" />
<img width="610" height="315" alt="image" src="https://github.com/user-attachments/assets/5a0e1026-8dda-41ee-afe9-5a9c3c419e6a" />
<img width="191" height="128" alt="image" src="https://github.com/user-attachments/assets/9937e0d1-5d18-4a13-9bd8-ac35e810ce84" />
<img width="191" height="128" alt="image" src="https://github.com/user-attachments/assets/03c5f9e0-2128-4457-b664-659fe7e06997" />

-----
# LOBBY WELCOME MESSAGE

```
!welcome-message TECH CORE PATCH Instructions https://github.com/Cebolletoth/TechCore-Patch-BAR/blob/main/TechCoreBAR.md      -T1 Cons can produce the Tech Core building, found on the Lab menu (Repurposed Experimental Armada Airlab).  -Tech Core building  (1TechPoint - Stats 1kM 10kE 10kBT 3kHP, +100E/s. It can be built on land or sea and it produces Tech Con (Repurposed Cortex Printer). -Tech Con (HOVER movement, 55speed, 350M 6.5kE, 10kBT +20E/s) only buildoption is to produce Tech Mexes -Repurposed Legion overcharged mex-. -Tech Mex (Stats 750M 8kE 12kBuildtime x3M income 30E/s upkeep). -T2 labs have partially reduced costs.
```

-----

-----
Feedback on testing parameters, unit/building costing and quality of gameplay is highly appreciated to allow us to fine tune the balance across all game modes. Please also include replays/videos links whenever possible.

------

# TECH CORE PATCH NOTES 0.6.2

*Requires "Force Load All Units"*

*Requires tweakdef XP removal (1) and TC tweakunits in three parts (3)*

-T1 Cons can produce the Tech Core building, found on the Lab menu (Repurposed Experimental Armada Airlab).

-Tech Core building (Stats 1000M 10000E 10000Buildtime 3000HP, +100E/s production, can be built on land or sea, cannot be reclaimed), produces Tech Con (Repurposed Cortex Printer).

-Tech Con (Hover movement, 55speed, 350M 6.5kE, 10kBT +20E/s) only ability is to produce Tech Mexes (Repurposed Legion overcharged mex).

-Tech Mex (Stats 750M, 6500E, 12000Buildtime, x3M income, 30E/s upkeep).

-T2 labs have reduced costs as part of the cost has already been invested into building the necessary Tech Cores.

-Legion faction changes: legmex gives 90%M and +4E/s, construction turrets receive +10bp as compensation for not having special minifortifier t1.5mex.

-----

# PASSIVE XP REMOVAL TWEAK

```
!bset tweakdefs Zm9yIG5hbWUsIHVuaXREZWYgaW4gcGFpcnMoVW5pdERlZnMpIGRvCiAgICB1bml0RGVmLmN1c3RvbXBhcmFtcyA9IHVuaXREZWYuY3VzdG9tcGFyYW1zIG9yIHt9CiAgICB1bml0RGVmLmN1c3RvbXBhcmFtcy50ZWNoX3BvaW50c19nYWluID0gMAplbmQ
```
-----
# TC TWEAK 1/3

```
!bset tweakunits7 LS0xLzMgMC42LjIgVEMgUGF0Y2gKewogYXJtY2sgPSB7CiAgYnVpbGRvcHRpb25zID0gewogICBbMzFdID0gImFybWFwdDMiLAogICAgfSwKIH0sCiBhcm1jayA9IHsKICBidWlsZG9wdGlvbnMgPSB7CiAgIFszMV0gPSAiYXJtYXB0MyIsCiAgICB9LAogfSwKIGNvcmNrID0gewogIGJ1aWxkb3B0aW9ucyA9IHsKICAgWzMxXSA9ICJhcm1hcHQzIiwKICAgIH0sCiB9LAogbGVnY2sgPSB7CiAgYnVpbGRvcHRpb25zID0gewogICAibGVnc29sYXIiLAogICAibGVnYWR2c29sIiwKICAgImxlZ3dpbiIsCiAgICJsZWdnZW8iLAogICAibGVnbXN0b3IiLAogICAibGVnZXN0b3IiLAogICAibGVnbWV4IiwKICAgIiIsCiAgICJsZWdlY29udiIsCiAgICJsZWdhbGFiIiwKICAgImxlZ2xhYiIsCiAgICJsZWd2cCIsCiAgICJsZWdhcCIsCiAgICJsZWdocCIsCiAgICJsZWduYW5vdGMiLAogICAibGVnZXllcyIsCiAgICJsZWdyYWQiLAogICAibGVnZHJhZyIsCiAgICJsZWdkdHIiLAogICAibGVnbGh0IiwKICAgImxlZ21nIiwKICAgImxlZ2NsdXN0ZXIiLAogICAibGVncmwiLAogICAibGVncmhhcHNpcyIsCiAgICJsZWdsdXBhcmEiLAogICAibGVnY3RsIiwKICAgImxlZ2phbSIsCiAgICJsZWdqdW5vIiwKICAgImNvcnN5IiwKICAgImxlZ2hpdmUiLAogICBbMzFdID0gImFybWFwdDMiLAogIH0sCiB9LAogYXJtY3YgPSB7CiAgYnVpbGRvcHRpb25zID0gewogICBbMzFdID0gImFybWFwdDMiLAogICAgfSwKIH0sCiBjb3JjdiA9IHsKICBidWlsZG9wdGlvbnMgPSB7CiAgIFszMV0gPSAiYXJtYXB0MyIsCiAgfSwKIH0sCiBsZWdjdiA9IHsKICBidWlsZG9wdGlvbnMgPSB7CiAgICJsZWdzb2xhciIsCiAgICJsZWdhZHZzb2wiLAogICAibGVnd2luIiwKICAgImxlZ2dlbyIsCiAgICJsZWdtc3RvciIsCiAgICJsZWdlc3RvciIsCiAgICJsZWdtZXgiLAogICAiIiwKICAgImxlZ2Vjb252IiwKICAgImxlZ2F2cCIsCiAgICJsZWdsYWIiLAogICAibGVndnAiLAogICAibGVnYXAiLAogICAibGVnaHAiLAogICAibGVnbmFub3RjIiwKICAgImxlZ2V5ZXMiLAogICAibGVncmFkIiwKICAgImxlZ2RyYWciLAogICAibGVnZHRyIiwKICAgImxlZ2xodCIsCiAgICJsZWdtZyIsCiAgICJsZWdjbHVzdGVyIiwKICAgImxlZ3JsIiwKICAgImxlZ3JoYXBzaXMiLAogICAibGVnbHVwYXJhIiwKICAgImxlZ2N0bCIsCiAgICJsZWdqYW0iLAogICAibGVnanVubyIsCiAgICJjb3JzeSIsCiAgICJsZWdoaXZlIiwKICAgWzMxXSA9ICJhcm1hcHQzIiwKICB9LAogfSwKIGFybWNhID0gewogIGJ1aWxkb3B0aW9ucyA9IHsKICAgWzMxXSA9ICJhcm1hcHQzIiwKICB9LAogfSwKIGNvcmNhID0gewogIGJ1aWxkb3B0aW9ucyA9IHsKICAgWzMxXSA9ICJhcm1hcHQzIiwKICB9LAogfSwKIGxlZ2NhID0gewogIGJ1aWxkb3B0aW9ucyA9IHsKICAgImxlZ3NvbGFyIiwKICAgImxlZ2FkdnNvbCIsCiAgICJsZWd3aW4iLAogICAibGVnZ2VvIiwKICAgImxlZ3V3Z2VvIiwKICAgImxlZ21zdG9yIiwKICAgImxlZ2VzdG9yIiwKICAgImxlZ21leCIsCiAgICIiLAogICAibGVnZWNvbnYiLAogICAiY29yYXNwIiwKICAgImNvcmZhc3AiLAogICAibGVnYWFwIiwKICAgImxlZ2xhYiIsCiAgICJsZWd2cCIsCiAgICJsZWdhcCIsCiAgICJsZWdocCIsCiAgICJsZWduYW5vdGMiLAogICAibGVnZXllcyIsCiAgICJsZWdyYWQiLAogICAibGVnZHJhZyIsCiAgICJsZWdkdHIiLAogICAibGVnbGh0IiwKICAgImxlZ21nIiwKICAgImxlZ2NsdXN0ZXIiLAogICAibGVncmwiLAogICAibGVncmhhcHNpcyIsCiAgICJsZWdsdXBhcmEiLAogICAibGVnY3RsIiwKICAgImxlZ2phbSIsCiAgICJsZWdqdW5vIiwKICAgImNvcnN5IiwKICAgImxlZ2hpdmUiLAogICBbMzRdID0gImFybWFwdDMiLAogIH0sCiB9LAp9
```
-----

# TC TWEAK 2/3

```
!bset tweakunits8 LS0yLzMgMC42LjIgVEMgUGF0Y2gKewogYXJtYWxhYiA9IHsKICBlbmVyZ3ljb3N0ID0gMTAwMDAsCiAgbWV0YWxjb3N0ID0gMTgwMCwKICBidWlsZHRpbWUgPSAxODAwMCwKIH0sCiBjb3JhbGFiID0gewogIGVuZXJneWNvc3QgPSAxMDAwMCwKICBtZXRhbGNvc3QgPSAxODAwLAogIGJ1aWxkdGltZSA9IDE4MDAwLAogfSwKIGxlZ2FsYWIgPSB7CiAgZW5lcmd5Y29zdCA9IDEwMDAwLAogIG1ldGFsY29zdCA9IDE4MDAsCiAgYnVpbGR0aW1lID0gMTgwMDAsCiB9LAogYXJtYXZwID0gewogIGVuZXJneWNvc3QgPSAxMDAwMCwKICBtZXRhbGNvc3QgPSAxOTUwLAogIGJ1aWxkdGltZSA9IDE5NTAwLAogfSwKIGNvcmF2cCA9IHsKICBlbmVyZ3ljb3N0ID0gMTAwMDAsCiAgbWV0YWxjb3N0ID0gMTk1MCwKICBidWlsZHRpbWUgPSAxOTUwMCwKIH0sCiBsZWdhdnAgPSB7CiAgZW5lcmd5Y29zdCA9IDEwMDAwLAogIG1ldGFsY29zdCA9IDE5NTAsCiAgYnVpbGR0aW1lID0gMTk1MDAsCiB9LAogYXJtYWFwID0gewogIGVuZXJneWNvc3QgPSAxMTAwMCwKICBtZXRhbGNvc3QgPSAyMTAwLAogIGJ1aWxkdGltZSA9IDIxMDAwLAogfSwKIGNvcmFhcCA9IHsKICBlbmVyZ3ljb3N0ID0gMTEwMDAsCiAgbWV0YWxjb3N0ID0gMjEwMCwKICBidWlsZHRpbWUgPSAyMTAwMCwKIH0sCiBsZWdhYXAgPSB7CiAgZW5lcmd5Y29zdCA9IDExMDAwLAogIG1ldGFsY29zdCA9IDIxMDAsCiAgYnVpbGR0aW1lID0gMjEwMDAsCiB9LAogYXJtYXN5ID0gewogIGVuZXJneWNvc3QgPSAxMTAwMCwKICBtZXRhbGNvc3QgPSAyNzAwLAogIGJ1aWxkdGltZSA9IDI3MDAwLAogfSwKIGNvcmFzeSA9IHsKICBlbmVyZ3ljb3N0ID0gMTEwMDAsCiAgbWV0YWxjb3N0ID0gMjcwMCwKICBidWlsZHRpbWUgPSAyNzAwMCwKIH0sCiBhcm1hY2sgPSB7CiAgc3BlZWQgPSA0MCwKIH0sCiBjb3JhY2sgPSB7CiAgc3BlZWQgPSA0MCwKIH0sCiBsZWdhY2sgPSB7CiAgc3BlZWQgPSA0MCwKIH0sCn0
```

-----

# TC TWEAK 3/3

```
!bset tweakunits9 LS0zLzMgMC42LjIgVEMgUGF0Y2gKewphcm1hcHQzID0gewogIGFjdGl2YXRld2hlbmJ1aWx0ID0gdHJ1ZSwKICBlbmVyZ3ljb3N0ID0gOTAwMCwKICBtZXRhbGNvc3QgPSAxMDAwLAogIGJ1aWxkZXIgPSB0cnVlLAogIGJ1aWxkcGljID0gIkFSTUFQLkREUyIsCiAgYnVpbGR0aW1lID0gMTAwMDAsCiAgY2FubW92ZSA9IHRydWUsCiAgY2FucmVwZWF0ID0gdHJ1ZSwKICByZWNsYWltYWJsZSA9IGZhbHNlLAogIGZvb3RwcmludHggPSA5LAogIGZvb3RwcmludHogPSA2LAogIGhlYWx0aCA9IDMwMDAsCiAgbWF4c2xvcGUgPSAxNSwKICBtYXh3YXRlcmRlcHRoID0gMTAwMCwKICBtZXRhbHN0b3JhZ2UgPSA1MDAsCiAgd29ya2VydGltZSA9IDMwMCwKICBlbmVyZ3ltYWtlID0gMTAwLAogIGJ1aWxkb3B0aW9ucyA9IHsKICAgWzFdID0gImNvcnByaW50ZXIiLAogICBbMl0gPSAiZmFsc2UiLAogICBbM10gPSAiZmFsc2UiLAogICBbNF0gPSAiZmFsc2UiLAogIH0sCiAgY3VzdG9tcGFyYW1zID0gewogICB1bml0Z3JvdXAgPSAnYnVpbGRlcicsCiAgIHRlY2hsZXZlbCA9IDEsCiAgIHRlY2hfY29yZV92YWx1ZSA9IDEsCiAgfSwKICBmZWF0dXJlZGVmcyA9IHsKICAgZGVhZCA9IHsKICAgIG1ldGFsID0gMjUwLAogICB9LAogICBoZWFwID0gewogICAgbWV0YWwgPSAzNTAsCiAgIH0sCiAgfSwKIH0sCmNvcnByaW50ZXIgPSB7CiAgICAgICAgY2FubW92ZSA9IHRydWUsCiAgICAgICAgYXV0b2hlYWwgPSA1LAogICAgICAgIGJ1aWxkZGlzdGFuY2UgPSAxMDAsCiAgICAgICAgYnVpbGRlciA9IHRydWUsCiAgICAgICAgYnVpbGR0aW1lID0gMTAwMDAsCiAgICAgICAgZW5lcmd5Y29zdCA9IDY1MDAsCiAgICAgICAgZW5lcmd5bWFrZSA9IDIwLAogICAgICAgIGVuZXJneXN0b3JhZ2UgPSA1MCwKICAgICAgICBtZXRhbGNvc3QgPSAzNTAsCiAgICAgICAgaGVhbHRoID0gOTAwLAogICAgICAgIHNpZ2h0ZGlzdGFuY2UgPSA0MzAsCiAgICAgICAgbW92ZW1lbnRjbGFzcyA9ICJIT1ZFUjMiLAogICAgICAgIHNwZWVkID0gNTUsCiAgICAgICAgbGVhdmV0cmFja3MgPSBmYWxzZSwKICAgICAgICB3b3JrZXJ0aW1lID0gMjAwLAogICAgICAgIGNhbnRiZXRyYW5zcG9ydGVkID0gdHJ1ZSwKICAgICAgICBidWlsZG9wdGlvbnMgPSB7CiAgICAgICAgICAgIFsxXSA9ICJsZWdtZXh0MTUiLAogICAgICAgICAgICBbMl0gPSAiZmFsc2UiLAogICAgICAgICAgICBbM10gPSAiZmFsc2UiLAogICAgICAgICAgICBbNF0gPSAiZmFsc2UiLAogICAgICAgIH0sCiAgICAgICAgY3VzdG9tcGFyYW1zID0gewogICAgICAgICAgICB0ZWNobGV2ZWwgPSAxLAogICAgICAgICAgICB1bml0Z3JvdXAgPSAiYnVpbGRlcnQxIiwKICAgICAgICB9LAogICAgfSwKIGxlZ21leHQxNSA9IHsKICBlbmVyZ3ljb3N0ID0gODAwMCwKICBtZXRhbGNvc3QgPSA3NTAsCiAgYnVpbGR0aW1lID0gMTIwMDAsCiAgZW5lcmd5dXBrZWVwID0gMzAsCiAgZXh0cmFjdHNtZXRhbCA9IDAuMDAzLAogIGhlYWx0aCA9IDI1MDAsCiAgbWV0YWxzdG9yYWdlID0gMjAwLAogIGZlYXR1cmVkZWZzID0gewogICBkZWFkID0gewogICAgZGFtYWdlID0gMTAwMCwKICAgIG1ldGFsID0gMzAwLAogICB9LAogICBoZWFwID0gewogICAgZGFtYWdlID0gNTAwLAogICAgbWV0YWwgPSAxNTAsCiAgIH0sCiAgfSwKIH0sCiBsZWduYW5vdGMgPSB7CiAgd29ya2VydGltZSA9IDIxMCwKIH0sCiBsZWdtZXggPSB7CiAgZW5lcmd5dXBrZWVwID0gLTQsCiAgZXh0cmFjdHNtZXRhbCA9IDAuMDAwOSwKfSwKfQ
```
