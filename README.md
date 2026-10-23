# Benjamin Shyong

**San Francisco** | **Ex-Apple, ex-Meta hardware** | **Building digital twins for hardware manufacturing**

<p>
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img alt="MuJoCo" src="https://img.shields.io/badge/MuJoCo-1F2937?style=flat-square">
  <img alt="NVIDIA" src="https://img.shields.io/badge/NVIDIA-76B900?style=flat-square&logo=nvidia&logoColor=white">
  <img alt="Next.js" src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white">
  <img alt="MCP/A2A" src="https://img.shields.io/badge/MCP%2FA2A-7C3AED?style=flat-square">
  <img alt="Codex" src="https://img.shields.io/badge/Codex-412991?style=flat-square&logo=openai&logoColor=white">
  <img alt="Claude" src="https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white">
</p>

> Simulation shows you what a design should do. A digital twin grounded in real-world physics and correlated to actual performance shows you what it actually does.

I spent ten years taking consumer hardware from prototype to mass production at Apple and Meta. In 2026 I left Meta to build full time.

## Now

I'm building digital twins of real manufacturing floors: the actual stations, fixtures and tolerances, modeled in physics and checked against what the line really produces. Hardware teams can then run the next prototype build virtually. They change a part, rerun thousands of units in minutes, and see the effect on yield and reliability before the next EVT or DVT. Every real build the model is checked against makes it more accurate.

- **Why:** at Apple (iPad Pro NPI, special projects, soft goods) and Meta (manufacturing readiness for Ray-Ban Display), a major build issue cost weeks of slip, and nobody found it until the parts existed.
- **Proof so far:** a Monte Carlo plus MuJoCo yield model of a snap-fit assembly. A 0.5 mm hook change moved predicted yield from 82.8% to 96.2%. The two models agree 98.4% of the time away from the pass/fail boundary, and the boundary is where real line data matters. An agentic version, [Factory N+1](https://github.com/benikigai/factory-n1), won **NVIDIA Best Use of Nemotron** at the Recursive Agents Hackathon (Oct 2026).
- **Stage:** early. I'm talking with NPI, DFX and manufacturing engineers about how their builds actually go.

**I'd like to talk to:**
- **Sim-to-real people:** contact-rich physics, robotics or line simulation (MuJoCo, Isaac, Omniverse, Genesis), and experience correlating a model with real hardware data.
- **Hardware teams** with a build coming up who would try a virtual one first.

Reach me through [benjaminshyong.com](https://benjaminshyong.com).

## Background

- **Meta and Apple (≈10 years):** consumer hardware NPI from prototype to mass production, with a lot of time on factory floors in China.
- **Lincoln Electric:** supply chain, ERP and factory systems. Systems and industrial engineering degree from Purdue.
- **[Injester](https://injester.com) (2026):** agent-native commerce for Shopify sellers, covering catalog to checkout, attribution and recovery. It started as a 1st-place build at Nebius.Build SF.

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
