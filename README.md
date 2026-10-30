# Benjamin Shyong

**San Francisco** | **17 years in hardware manufacturing (Apple, Meta)** | **Founder, N+1 Labs**

<p>
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img alt="MuJoCo" src="https://img.shields.io/badge/MuJoCo-1F2937?style=flat-square">
  <img alt="OpenUSD" src="https://img.shields.io/badge/OpenUSD-0F766E?style=flat-square">
  <img alt="NVIDIA" src="https://img.shields.io/badge/NVIDIA-76B900?style=flat-square&logo=nvidia&logoColor=white">
  <img alt="Next.js" src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white">
  <img alt="MCP/A2A" src="https://img.shields.io/badge/MCP%2FA2A-7C3AED?style=flat-square">
  <img alt="Codex" src="https://img.shields.io/badge/Codex-412991?style=flat-square&logo=openai&logoColor=white">
  <img alt="Claude" src="https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white">
</p>

> Most teams building AI for factories are software people learning manufacturing. I'm the reverse. I've spent 17 years on factory floors, and now I build the software myself with coding agents.

## Now: N+1 Labs

N+1 Labs predicts where a hardware team's next factory build will fail, before tooling, fixtures and the line are committed.

Every factory has three versions:
- **N−1:** the line rebuilt from a teardown of a shipped product
- **N:** the line you run
- **N+1:** your next build, simulated first

The engine models the real stations, fixtures and tolerances in physics (Monte Carlo plus MuJoCo, on CPU), runs thousands of virtual units in minutes, and ranks what will fail. The hard part is the loop: score each prediction against a real build, then recalibrate until the twin earns a Proven grade. Nothing is scored on a real build yet. A blind backtest on a past build comes first.

- **Why:** at Apple (iPad Pro NPI, special projects, soft goods) and Meta (Ray-Ban Display), a major build issue cost weeks of slip, and nobody found it until the parts existed. What one program learned lived in slide decks, so the next team learned it again.
- **Proof so far:** a Monte Carlo plus MuJoCo yield model of a synthetic snap-fit part. A 0.5 mm hook change moved simulated yield from 82.76% to 96.24%, with 5,000 virtual units in about 5.5 seconds on one workstation. An agentic version, [Factory N+1](https://github.com/benikigai/factory-n1), won **NVIDIA Best Use of Nemotron** at the Recursive Agents Hackathon (Oct 2026).

## Open Product

GitHub opened up code. Hugging Face opened up AI models. Open Product opens up hardware.

Each release is an OPD (Open Product Description), built on OpenUSD and STEP: the bill of materials, supply chain, station layout, fixtures and every assembly step for a shipped product, in one package. OPDs can be public or private, and private ones can go public after an embargo. First release: Nintendo Joy-Con, December 2026.

## I'd like to talk to

- **Sim-to-real people:** contact-rich physics, robotics or line simulation (MuJoCo, Isaac, Omniverse, Genesis), with experience correlating a model to real hardware data. I'm looking for a co-founder here.
- **Hardware teams** with a past build they'd let us blind-backtest, or a build coming up they'd try virtually first.
- **Teardown and hardware people** who want to help write the first OPDs.

Reach me through [benjaminshyong.com](https://benjaminshyong.com).

## Background

- **Meta (2022 to 2026):** Staff TPM. Led Ray-Ban Display, the first consumer glasses with a monocular AR display, from prototype to mass production, then Ray-Ban Meta audio glasses.
- **Apple (2016 to 2022):** took iPad Pro from prototype to mass production, stood up a new manufacturer and automation line for a health product, and ran operations and quality on iPhone.
- **Lincoln Electric (2009 to 2016):** manufacturing engineering to operations lead, ending with an ERP rollout across five China plants.
- 9 factory cities across China, Vietnam and Taiwan. Systems and industrial engineering, Purdue.
- **[Injester](https://injester.com) (2026):** co-founded agent-native commerce for Shopify sellers, which started as a 1st-place build at Nebius.Build SF. I'm now full-time on N+1 Labs.

## 2026 hackathons

I build in the open at hackathons, usually solo or with a small team, and ship working demos in a day. Wins:

| Result | Event | Build |
|---|---|---|
| 🥇 NVIDIA Best Use of Nemotron | Recursive Agents Hackathon (Crusoe), Oct 2026 | [Factory N+1](https://github.com/benikigai/factory-n1): Nemotron agents redesign a fulfillment floor, and a change ships only if it wins on unseen days |
| 🥇 1st place | Cerebral Valley × Rosewood Hospitality 2030, May 2026 | [Red Thread](https://github.com/benikigai/redthread): agent OS for luxury hospitality with live hotel-to-guest A2A handoff |
| 🥇 1st place | DataHub × Nebius, Apr 2026 | [data-oncall](https://github.com/benikigai/datahub-hackathon-oncall): 4 agents use lineage to find the root cause of data incidents in about 90 s |
| 🥇 1st place | Nebius.Build SF, Mar 2026 | [Injester](https://injester.com): agent-commerce prototype that became Injester |
| Top-six finalist | YC Agent Hack Day (AWS Builder Loft), Apr 2026 | [LoopOS](https://github.com/benikigai/loopos): MCP-native back-office agent for service operations |

<details>
<summary>All the other builds</summary>

- [Marginalia](https://github.com/benikigai/marginalia): on-device voice agent for smart glasses (Gemma 4 + Even Realities G2, zero cloud). YC Gemma 4 Voice.
- [Timbre](https://github.com/benikigai/timbre): two Gemini agents argue so a founder's voice survives. Google I/O.
- [Scriber](https://github.com/benikigai/scriber): meeting agent that runs your standup live and edits Linear mid-call. OpenAI Voice Hack Night.
- [reSKILL](https://github.com/benikigai/reSKILL): sealed replay gate for self-improving agent skills. AI Engineer World's Fair.
- [WorldKinetics](https://github.com/benikigai/worldkinetic): customize everyday products without CAD; the model writes the CAD and independent checks gate approval. OpenAI GPT-6 Astra.
- [AgentMES](https://github.com/benikigai/agent-mes): agents do the work and humans own the gates in a 7-stage engineering workflow. Blaxel × Codex × Redis.
- [DarkMesh](https://github.com/benikigai/darkmesh): resilient edge sensor-fusion mesh for disconnected environments. National Security Hackathon.
- [AgentTalkie](https://github.com/benikigai/agenttalkie), [JEVgotiator](https://github.com/benikigai/JEVgotiator), [Corgi Ads](https://github.com/benikigai/corgihack): voice agent workspace, used-Tesla negotiation agent, ad agent with human-approved spend.

</details>

## What I run day to day

I run an agent fleet on my own hardware, and it does a lot of my real work:

- 🌙 **[Nightshift](https://github.com/benikigai/nightshift):** Ralph-loop agent harness with build, gate, separate evaluator, retry and commit. Its public proof run built 29 of 30 features for about $0.95.
- 🦾 **[Elias](https://github.com/benikigai/elias):** my OpenClaw assistant, with specialized agents, multiple channels, versioned memory and local inference on a home GPU and DGX Spark cluster.
- 🧰 **[TurnkeyHost](https://preview.turnkeyhost.ai) and [Stay Ikigai](https://stayikigai.com):** a self-hosted PMS that runs my five short-term rentals (reservations, guest messages, cleaning, pricing). The live testbed for everything above.
- 🧭 **[Agent Web Protocol](https://agentwebprotocol.org):** an open discovery spec for what agents can do on a web surface.
