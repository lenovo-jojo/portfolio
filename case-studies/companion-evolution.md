# JARVIS / Critter Comforts — companion evolution

## The idea

Explore a companion that feels present in an interactive environment, rather than only inside a chat window. The project has taken several forms as I explored character interaction, dialogue, memory, movement, and presentation.

## Iterations and evidence

| Iteration | Direction | Evidence and status |
| --- | --- | --- |
| Desktop pet | A companion that lives alongside everyday computer use | Part of my project history; the original source/demo is still being located. |
| GameCube dialogue mod | Connect model-generated dialogue to Animal Crossing in Dolphin | Python source includes dialogue parsing/encoding, memory readers, conversation-state tracking, and a choice-menu injection test. [Recovered Python source and three passing dialogue checks](https://github.com/lenovo-jojo/Jarvis/tree/main/examples/gamecube-dialogue) are public. An end-to-end emulator demo has not been verified in this portfolio pass. |
| JavaScript / browser | Explore a companion/world through web technologies | [Recovered Three.js/TypeScript source](https://github.com/lenovo-jojo/Jarvis/tree/main/examples/browser-world) is public and passes typecheck and production build. It includes player/camera controllers, procedural world modules, and authored scene data. Runtime rendering still needs separate verification. |
| Unity / JARVIS | A local-first 3D companion prototype using C#, VRM avatars, and an OpenAI-compatible local endpoint | [Public Unity source](https://github.com/lenovo-jojo/Jarvis) imports and compiles. Pose-discovery checks found 18 standard poses without optional content and 27 with it installed. Original personal avatars are excluded; full scene playback remains unverified. |

## An engineering decision: optional content boundaries

As the prototype grew, optional content became coupled to core pose loading. I separated the inspected optional pose pack from the public core, preserved its metadata and verified copies privately, and replaced the hardcoded pack location with a generic optional-content path. Both pose-discovery configurations were checked in Unity. Original models and historical private material remain outside the public repository.

The remaining epic work is a visible avatar/scene demonstration and a complete standalone-player add-on workflow. Discovery and compilation are verified; full animation playback is not.

## My role

I originated and directed the companion experience, iterated on product and scene behavior, and developed it with AI assistance. I am documenting the implemented systems and tradeoffs rather than treating every prototype idea as a shipped capability.

## What this demonstrates

The project provides material for discussing integration boundaries, stateful interactions, avatar/animation backends, local service configuration, and how prototypes inform later design choices. A technical reviewer should distinguish inspected source from demonstrated runtime behavior; more runtime evidence is being prepared. [The source-example CI passed](https://github.com/lenovo-jojo/Jarvis/actions/runs/38209453135).
