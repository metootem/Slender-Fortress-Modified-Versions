Personal fork of SF2M 1.8.0 Alpha 2.73d featuring some fixes and changes. Everything is done for specific circumstances

Some of the changes include (sorted by first created from top in each category):

## Core

Added ConVar sf2_disallow_boss_music<br/>
Added ConVar sf2_disallow_page_music<br/>
Added NetProp sf2_szCustomEscapeMessage to sf2_gamerules<br/>
Added NetProp sf2_szCustomPageMessage to sf2_gamerules<br/>
Added Native SF2_GetMaxPages<br/>
Added Native SF2_RevealPages<br/>
Added Forward SF2_OnRoundTimeCount<br/>
Added Forward SF2_OnEscapeTimeCount<br/>
Added Native SF2_GetRoundTimeCount<br/>
Added chat message hint for /slupdate<br/>
Added Revenant boss pack fallback if there were no revenant bosses loaded<br/>
Added ConVar sf2_revenant_wave_time<br/>
Changed Music System to always play on the music channel<br/>

## SF2_Player

Added SF2_player PluginSprintSpeed property<br/>
Added SF2_Player PluginWalkSpeed property<br/>
Added Forward SF2_OnClientPreInstantKill<br/>
Added SF2_Player StaticDisabled property<br/>
Added SF2_Player AntiCamping property<br/>
Added SF2_Player StatsHUD property<br/>
Added SF2_Player TimerHUD property<br/>
Added Forward SF2_OnClientAntiCampingStrike<br/>
Disabled Player Dynamic FOV<br/>
Added Forward SF2_OnClientMusicStart<br/>
Added Forward SF2_OnClientMusicStop<br/>
Added Native SF2_IsClientMusicPlaying<br/>
Added SF2_player CanCollideWithBosses property<br/>
Added Native SF2_GetClientUltravisionEnt<br/>

## Bosses

Added Forward SF2_OnBossPreAdded<br/>
Added Forward SF2_OnSlenderVisionTraceEntity<br/>
Added Forward SF2_OnSlenderAttackTraceEntity<br/>
Added Native SF2_SetBossStunnable<br/>
Added Native SF2_GetBossForceStunnable<br/>
Added Native SF2_SetBossStunDisappear<br/>
Added Native SF2_GetBossForceStunDisappear<br/>
Added Native SF2_SetBossForceGlow<br/>
Added Native SF2_GetBossForceGlow<br/>
Added Native SF2_SetBossForcedTeleport<br/>
Added Native SF2_SetBossTeleportIgnoreVis<br/>
Added Native SF2_SetBossTeleportIgnoreChases<br/>
Added Native SF2_SetBossTeleportMin<br/>
Added Native SF2_SetBossTeleportMax<br/>
Fixed bosses always picking the same target at beginning of a round<br/>
Fixed all bosses removing their teleport target when at least 1 player has stress above any active boss threshold<br/>
Changed "teleport_ignore_chases" checking if only the teleport target is being chased instead of any player<br/>
Changed boss teleport and target selection system<br/>
Added boss config key "teleport_target_max_targeted"<br/>
Added boss config key "teleport_target_ignore_targeted"<br/>
Added Native SF2_SetBossIgnoreTargeted<br/>
Added Native SF2_SetCustomDifficultyString<br/>
Added flashlight stun check for entity collision group 1<br/>
Added boss config key "run_yawrate" for run attacks<br/>

### and maybe more that haven't been documented