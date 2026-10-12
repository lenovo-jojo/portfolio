# JARVIS / Critter Comforts — companion evolution

## The idea

Explore a companion that feels present in an interactive environment, rather than only inside a chat window. The project has taken several forms as I explored character interaction, dialogue, memory, movement, and presentation.

## Iterations and evidence

| Iteration | Direction | Evidence and status |
| --- | --- | --- |
| Desktop pet | A companion that lives alongside everyday computer use | Part of my project history; the original source/demo is still being located. |
| GameCube dialogue mod | Connect model-generated dialogue to Animal Crossing in Dolphin | Python source includes dialogue parsing/encoding, memory readers, conversation-state tracking, and a choice-menu injection test. Source publication is undergoing cleanup; an end-to-end emulator demo has not been verified in this portfolio pass. |
| JavaScript / browser | Explore a companion/world through web technologies | A project iteration; the exact source and deployable demo are still being organized. The separate Neocities site demonstrates my web experimentation. |
| Unity / JARVIS | A local-first 3D companion prototype using C#, VRM avatars, and an OpenAI-compatible local endpoint | Source inspection confirms service separation for model requests, avatar backends, voice, UI, camera, and memory. Source publication and a repeatable demonstration remain in progress. |

## An engineering decision: optional content boundaries

As the prototype grew, optional content became coupled to core pose loading. I am separating optional private assets from the public core so a public checkout can work without private dependencies. This requires dependency review, preserving Unity asset GUIDs, checking both configurations, and cleaning historical content before publication.

That work is tracked as an ongoing epic. It is not claimed as a completed or runtime-verified feature.

## My role

I originated and directed the companion experience, iterated on product and scene behavior, and developed it with AI assistance. I am documenting the implemented systems and tradeoffs rather than treating every prototype idea as a shipped capability.

## What this demonstrates

The project provides material for discussing integration boundaries, stateful interactions, avatar/animation backends, local service configuration, and how prototypes inform later design choices. A technical reviewer should distinguish inspected source from demonstrated runtime behavior; more runtime evidence is being prepared.
