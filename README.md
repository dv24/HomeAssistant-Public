# HomeAssistant Public

Home Assistant automations I'm happy to share. Each file starts with a comment listing the
entities and integrations it needs. Entity IDs and the notify target are placeholders:
replace them with your own before use.

| Automation | What it does |
|---|---|
| [office_lighting_lux.yaml](automations/office_lighting_lux.yaml) | Sets office light brightness and colour temperature from ambient lux, detects manual changes and backs off, clears the override at set times. 4 automations. |
| [battery_replacement_reminder.yaml](automations/battery_replacement_reminder.yaml) | Daily phone notification listing low batteries (Battery Notes), with a "Replaced" button per device. |
| [appliance_cycle_notifications.yaml](automations/appliance_cycle_notifications.yaml) | Washer and tumble drier cycle detection from smart-plug power, with live "running" and "finished" notifications. |
| [mute_speakers_while_coldplay_plays.yaml](automations/mute_speakers_while_coldplay_plays.yaml) | Silences speakers while the current artist is Coldplay and restores them afterwards. Mutes Music Assistant players; for AirPlay-started playback it saves the volume, drops it to 0 and restores it. |
| [unifi_ap_memory_alert.yaml](automations/unifi_ap_memory_alert.yaml) | Alerts on UniFi AP memory above 90% for 30 minutes, or on the integration going dark. |
| [pause_speaker_during_teams_call.yaml](automations/pause_speaker_during_teams_call.yaml) | Pauses a speaker when Teams reports you're in a call. |

Notes: some files are a list of several automations, which you can paste into `automations.yaml`.
For the UI editor, paste one automation at a time via **Edit in YAML**. Radio and artist-based
automations depend on the stream sending metadata, so a few seconds at either end can leak through.
