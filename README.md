# HomeAssistant Public

Home Assistant bits I'm happy to share.

## Automations

- [Mute speakers while Coldplay plays](automations/mute_speakers_while_coldplay_plays.yaml) —
  mutes any Music Assistant speaker whose current artist contains "Coldplay" and unmutes it
  when the artist changes or playback stops. Edit the `media_player` entity list to match your speakers.

Note: the artist only updates when the stream sends metadata, so a few seconds at either end of a
radio track can leak through.
