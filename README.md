# OpenAI Agents API: Labs 01–12

This React and Node app introduces the OpenAI Agents API through twelve hands-on labs. The Node server keeps the API key private and streams agent responses to the browser.

## Lab 01 — Create your first agent

Build a programming tutor with a model and instructions. Each question creates a new session, and the app displays the answer as events arrive. The lab introduces agents, sessions, turns, and streaming, with code explanations in the interface. See [LAB01.md](LAB01.md) for the implementation walkthrough and key code snippets.

## Lab 02 — Continue and customize

Ask follow-up questions in the same session so the tutor can use earlier messages as context. Then edit the tutor's instructions and start a new session to compare its answers. See [LAB02.md](LAB02.md) for the walkthrough.

## Lab 03 — Inspect the lifecycle

Use the live event inspector to compare session, turn, event, and saved item IDs, and read the turn outcome. See [LAB03.md](LAB03.md) for the exercise.

## Lab 04 — Handle interrupted work

Inspect API errors, cancellation, and a simulated stream disconnect. Retrieve saved session state before retrying. See [LAB04.md](LAB04.md) for the walkthrough.

## Lab 05 — Manage sessions

List, retrieve, and delete sessions in a paginated history view. The teaching section includes explained code snippets and Viva voice read-aloud controls. See [LAB05.md](LAB05.md) for the walkthrough.


## Lab 06 — Move to TypeScript

Run the typed tutor, inspect validated streamed events, and test a malformed event at the runtime boundary. The teaching section has four explained snippets and Viva voice read-aloud controls. See [LAB06.md](LAB06.md) for the walkthrough.

## Lab 07 — Save and reuse an agent

Create a named tutor preset, retrieve it after a reload, and use its `agent_id` for two new sessions. The teaching section has explained code snippets and Viva voice controls. See [LAB07.md](LAB07.md) for the walkthrough.

## Lab 08 — Override one session

Use the same saved agent for a baseline session and a session with appended instructions. Compare their results, then retrieve the saved preset to verify it is unchanged. The teaching section has explained code snippets and Viva voice controls. See [LAB08.md](LAB08.md) for the walkthrough.

## Lab 09 — Compare models and reasoning settings

Run the same setup and follow-up prompts in two sessions. Update one session's model and reasoning effort before its follow-up, then compare answers, latency, and available usage in a downloadable worksheet. The teaching section includes explained code snippets and Viva voice controls. See [LAB09.md](LAB09.md) for the walkthrough.

## Lab 10 — Design an output contract

Generate a study plan from a saved tutor preset, validate every field on the server, and inspect one repair attempt when output is malformed. An offline playground demonstrates both rejection and acceptance. The teaching section includes explained code snippets and Viva voice controls. See [LAB10.md](LAB10.md) for the walkthrough.

## Lab 11 — Render text events correctly

Stream one answer through a naive renderer and a keyed text buffer side by side. Deltas are kept per content part, replayed events are skipped, and each part is replaced by its completed text. A step-through replayer needs no API key and shows interleaved parts, commentary, and a replayed delta. The teaching section includes five explained snippets and Viva voice controls. See [LAB11.md](LAB11.md) for the walkthrough.

## Lab 12 — Build a turn timeline

Record every event of a live session as metadata and group it by turn: a session lane, one lane per root or subagent turn, and numbered events in arrival order. Send a follow-up to add a second turn to the same session. A step-through replayer needs no API key and shows text deltas without a `turn_id`, two turns in one session, a subagent turn inside the root turn, and a failed turn with replayed and late events. The teaching section includes six explained snippets and Viva voice controls. See [LAB12.md](LAB12.md) for the walkthrough.
