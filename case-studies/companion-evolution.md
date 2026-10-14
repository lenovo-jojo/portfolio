# jarvis / critter comforts — companion evolution

## the idea

explore a companion that feels present in an interactive environment, rather than only inside a chat window. the project has taken several forms as i explored character interaction, dialogue, memory, movement, and presentation.

## iterations and evidence

| iteration | direction | evidence and status |
| --- | --- | --- |
| desktop pet | a companion that lives alongside everyday computer use | part of my project history; the original source/demo is still being located. |
| gamecube dialogue mod | connect model-generated dialogue to animal crossing in dolphin | python source includes dialogue parsing/encoding, memory readers, conversation-state tracking, and a choice-menu injection test. [recovered python source and three passing dialogue checks](https://github.com/lenovo-jojo/critter-comforts-cozy-cove/tree/main/examples/gamecube-dialogue) are public. an end-to-end emulator demo has not been verified in this portfolio pass. |
| javascript / browser | explore a companion/world through web technologies | [recovered three.js/typescript source](https://github.com/lenovo-jojo/critter-comforts-cozy-cove/tree/main/examples/browser-world) is public and passes typecheck and production build. it includes player/camera controllers, procedural world modules, and authored scene data. runtime rendering still needs separate verification. |
| unity / jarvis | a local-first 3d companion prototype using c#, vrm avatars, and an openai-compatible local endpoint | [public unity source](https://github.com/lenovo-jojo/critter-comforts-cozy-cove) imports and compiles. pose-discovery checks found 18 standard poses without optional content and 27 with it installed. original personal avatars are excluded; full scene playback remains unverified. |

## an engineering decision: optional content boundaries

as the prototype grew, optional content became coupled to core pose loading. i separated the inspected optional pose pack from the public core, preserved its metadata and verified copies privately, and replaced the hardcoded pack location with a generic optional-content path. both pose-discovery configurations were checked in unity. original models and historical private material remain outside the public repository.

the remaining epic work is a visible avatar/scene demonstration and a complete standalone-player add-on workflow. discovery and compilation are verified; full animation playback is not.

## my role

i originated and directed the companion experience, iterated on product and scene behavior, and developed it with ai assistance. i am documenting the implemented systems and tradeoffs rather than treating every prototype idea as a shipped capability.

## what this demonstrates

the project provides material for discussing integration boundaries, stateful interactions, avatar/animation backends, local service configuration, and how prototypes inform later design choices. a technical reviewer should distinguish inspected source from demonstrated runtime behavior; more runtime evidence is being prepared. [the source-example ci passed](https://github.com/lenovo-jojo/critter-comforts-cozy-cove/actions/runs/38209453135).
