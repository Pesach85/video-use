# Hub integration (video-use vendor)

## Secrets policy (MOCK / HITL)

- `elevenlabs_mode` in hub `config/cross_agent_media.json` is **`mock`**.
- Hub adapters **must not** call ElevenLabs APIs or write keys to hub `.env`.
- Real transcription is founder-HITL only, after an explicit yes and a non-hub secret store.

## Adapter

`src.agents.cross_agent_media.plan_release_video` + `mock_elevenlabs_transcribe`

Fork: https://github.com/Pesach85/video-use
