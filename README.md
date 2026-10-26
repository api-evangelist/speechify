# Speechify (speechify)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
