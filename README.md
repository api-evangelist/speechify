# Speechify (speechify)

Speechify is a text-to-speech platform whose Speechify Voice API (also surfaced through Speechify Studio) synthesizes lifelike speech in 30+ languages from plain text or SSML. The REST API at https://api.sws.speechify.com offers non-streaming and streaming text-to-speech, a voice catalog, and instant voice cloning, authenticated with a Bearer API key.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/apis.yml)

## Tags

- AI
- Text to Speech
- Voice
- Speech Synthesis
- Voice Cloning

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Speechify Text-to-Speech API

Synthesizes lifelike speech from plain text or SSML via POST /v1/audio/speech, returning base64-encoded audio (wav, mp3, ogg, aac, or pcm) plus speech marks for word-level timing, using the simba-english or simba-multilingual models across 30+ languages.

- **Human URL:** [https://docs.sws.speechify.com/v1/api-reference/api-reference/tts/audio/speech](https://docs.sws.speechify.com/v1/api-reference/api-reference/tts/audio/speech)
- **Base URL:** `https://api.sws.speechify.com/v1`

#### Tags

- Text to Speech
- Speech Synthesis
- SSML

#### Properties

- [Documentation](https://docs.sws.speechify.com/tts/overview/welcome)
- [API Reference](https://docs.sws.speechify.com/v1/api-reference/api-reference/tts/audio/speech)
- [OpenAPI](openapi/speechify-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/speechify.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/speechify.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Speechify Streaming TTS API

Streams synthesized audio as a chunked HTTP response from POST /v1/audio/stream for sub-300ms time-to-first-byte playback, with Accept values of audio/mpeg, audio/ogg, audio/aac, or audio/pcm (WAV is not available for streaming).

- **Human URL:** [https://docs.sws.speechify.com/v1/api-reference/api-reference/tts/audio/stream](https://docs.sws.speechify.com/v1/api-reference/api-reference/tts/audio/stream)
- **Base URL:** `https://api.sws.speechify.com/v1`

#### Tags

- Streaming
- Text to Speech
- Low Latency

#### Properties

- [Documentation](https://docs.sws.speechify.com/docs/features/streaming)
- [API Reference](https://docs.sws.speechify.com/v1/api-reference/api-reference/tts/audio/stream)
- [OpenAPI](openapi/speechify-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/speechify.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/speechify.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Speechify Voices API

Lists the available voices via GET /v1/voices, including 1,000+ pre-set Speechify voices and any personal cloned voices, each with id, gender, locale, and tags for selection by voice_id.

- **Human URL:** [https://docs.sws.speechify.com/v1/api-reference/api-reference/tts/voices](https://docs.sws.speechify.com/v1/api-reference/api-reference/tts/voices)
- **Base URL:** `https://api.sws.speechify.com/v1`

#### Tags

- Voices
- Catalog

#### Properties

- [Documentation](https://docs.sws.speechify.com/tts/overview/welcome)
- [API Reference](https://docs.sws.speechify.com/v1/api-reference/api-reference/tts/voices/delete)
- [OpenAPI](openapi/speechify-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/speechify.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/speechify.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Speechify Voice Cloning API

Creates an instant personal voice clone from a 10-30 second audio sample via multipart POST /v1/voices with explicit consent (full name and email), and removes cloned voices via DELETE /v1/voices/{id}.

- **Human URL:** [https://docs.sws.speechify.com/tts/guides/voice-cloning](https://docs.sws.speechify.com/tts/guides/voice-cloning)
- **Base URL:** `https://api.sws.speechify.com/v1`

#### Tags

- Voice Cloning
- Custom Voices

#### Properties

- [Documentation](https://docs.sws.speechify.com/v1/docs/features/voice-cloning)
- [API Reference](https://docs.sws.speechify.com/v1/api-reference/api-reference/tts/voices/delete)
- [OpenAPI](openapi/speechify-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/speechify.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/speechify.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/SpeechifyInc)
- [LinkedIn](https://www.linkedin.com/company/speechify)
- [Website](https://speechify.com)
- [Documentation](https://docs.sws.speechify.com)
- [Plans](plans/speechify-plans-pricing.yml)
- [Rate Limits](rate-limits/speechify-rate-limits.yml)
- [Fin Ops](finops/speechify-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
