# 2026 Research Update — AI Content Provenance & On-Chain IP

> **Scope of this update.** This repository's original thesis (2024–2025) was an **NFT marketplace for trading creative AI prompts**, with MOC as the currency. Between 2024 and mid-2026 the ground under that thesis shifted: the durable value moved *one layer down*, from the **prompt** to **provenance and licensing rights over the content itself.** This document reviews what changed and proposes a repositioning of the repo from "prompt-NFT marketplace" toward "**AI provenance + on-chain IP licensing infrastructure, settled in MOC.**"
>
> *Last reviewed: July 2026. Claims are dated and sourced inline; unverifiable items are marked and collected under "Open Questions & Caveats."*

---

## TL;DR

Between 2024 and 2026 the field pivoted from speculative "prompt NFT" marketplaces toward **hardened provenance and on-chain IP-licensing infrastructure.** Three forces drove it:

1. **Provenance went into production.** C2PA **Content Credentials** and Google **SynthID** moved from pilots to phones, cameras, creator tools, and frontier models.
2. **Labeling became law.** The **EU AI Act (Article 50)** makes machine-readable marking of AI-generated content legally required **from 2 August 2026.**
3. **IP went on-chain.** **Story** launched a Layer-1 turning IP into programmable, licensable assets — while a US Copyright Office ruling held that **a prompt alone is not an ownable authored work.**

Together these erode the "prompt-as-asset" premise and create real demand for **provenance + licensing rails** — a better fit for MOC.

---

## 1. What changed, 2024 → mid-2026

### 1.1 Provenance moved into production

- **OpenAI joined the C2PA Steering Committee (May 7, 2024)** alongside Adobe, BBC, Google, Intel, Microsoft, Publicis, Sony, and Truepic — committing to attach tamper-evident **Content Credentials** to generated media. This made C2PA the de-facto cross-industry provenance layer rather than a niche newsroom tool. ([c2pa.org](https://c2pa.org/openai-joins-c2pa-steering-committee/))
- **Adobe Content Authenticity web app — public beta (Apr 24, 2025).** A free tool letting creators attach, customize, and inspect Content Credentials — including a machine-readable **"do-not-train" generative-AI preference** — plus a Chrome inspection extension. Provenance and opt-out signals reached the long tail of creators. ([blog.adobe.com](https://blog.adobe.com/en/publish/2025/04/24/adobe-content-authenticity-now-public-beta-helps-creators-secure-attribution))
- **Google SynthID Detector (May 20, 2025).** A portal to detect SynthID watermarks across images, audio, video, and text from Gemini, Imagen, Lyria, and Veo; Google stated **10B+ pieces of content** had been watermarked since 2023. Watermark detection complements C2PA metadata for the case where metadata is stripped. ([blog.google](https://blog.google/innovation-and-ai/products/google-synthid-ai-content-detector/))
- **Provenance at the point of capture (2025).** Consumer smartphones began *signing* Content Credentials in-camera — e.g., Samsung Galaxy S25 (native camera) and Google Pixel 10 — moving authenticity from post-hoc editing tools onto mass-market devices. ([Pixel 10 — android.gadgethacks.com](https://android.gadgethacks.com/news/google-pixel-10-adds-c2pa-support-to-fight-ai-fakes/)) *(likely; device/firmware specifics from tech press)*
- The **C2PA spec matured (v2.2, ~May 2025)** with better video/cloud manifest handling. ([Content Credentials](https://en.wikipedia.org/wiki/Content_Credentials)) *(exact date should be confirmed against the C2PA changelog)*

### 1.2 Labeling became a legal requirement

- **EU AI Act Article 50 — from 2 August 2026.** Providers of generative systems must mark synthetic output in a **machine-readable, detectable format** (watermark/metadata), and deployers must disclose deepfakes and certain AI-generated public-interest text, with artistic/satirical exceptions. This turns provenance labeling from voluntary best-practice into hard legal demand. ([artificialintelligenceact.eu](https://artificialintelligenceact.eu/article/50/))
- **EU Code of Practice on Transparency of AI-Generated Content (2026).** The European Commission published guidance operationalizing Article 50, including an interim visible-label convention pending a standardized EU symbol. ([digital-strategy.ec.europa.eu](https://digital-strategy.ec.europa.eu/en/policies/code-practice-ai-generated-content)) *(date/scope from legal commentary; it is guidance, not binding law)*

### 1.3 IP went on-chain — and prompts lost their ownership claim

- **Story ("Story Protocol") — $80M Series B at $2.25B, led by a16z crypto (Aug 21, 2024); Layer-1 mainnet + IP token (Feb 2025).** Story is a purpose-built blockchain that registers works as on-chain **IP Assets** (ERC-721) with a **Programmable IP License (PIL)** linking on-chain smart contracts to off-chain legal terms, enabling automated royalties and derivative tracking ("**IPFi**"). ([techcrunch.com](https://techcrunch.com/2024/08/21/story-raises-83m-at-a-2-25b-valuation-to-build-a-blockchain-for-the-business-of-content-ip-in-the-age-of-ai/) · [decrypt.co](https://decrypt.co/305730/story-protocol-debuts-mainnet-with-1-billion-ip-tokens-to-claim)) *(mainnet date/network name from crypto press — confirm against primary source)*
- **US Copyright Office — prompts do not confer authorship (Jan 2025).** "Copyright and AI, Part 2: Copyrightability" concluded that fully AI-generated outputs lack human authorship and are not copyrightable, and that entering a prompt — however detailed — does not confer copyright; only perceptible human contributions are protectable, case-by-case. ([copyright.gov, PDF](https://www.copyright.gov/ai/Copyright-and-Artificial-Intelligence-Part-2-Copyrightability-Report.pdf))

This is the decisive blow to "prompt-as-ownable-asset": under US law, the prompt string itself is not the protectable thing.

### 1.4 The prompt-market itself split

- **PromptBase** persisted into 2026 as a conventional **Web2** prompt marketplace (no crypto/NFT model). ([tracxn.com](https://tracxn.com/d/companies/promptbase/__rwbBOyb3nk-QxJtJohphuSVEPTVAhLhUecHdSV8wFQ4)) *(likely)*
- **NFPrompt** (BNB Chain, launched 2023) remained active but reportedly **broadened away from pure prompt-NFT minting** toward AI trading/agent features. ([coinmarketcap.com](https://coinmarketcap.com/currencies/nfprompt/)) *(uncertain — pivot specifics from project self-reporting)*

**The signal:** the prompt-*marketplace* category survived as plain fiat commerce, while the specifically on-chain **"prompt NFT"** framing lost momentum. Value migrated to provenance and licensing.

---

## 2. Mossland's revised angle

The original repo — an NFT platform for trading creative AI prompts — sits on a thesis the 2024–2026 evidence has largely eroded (prompts aren't ownable authored works; surviving prompt marketplaces are Web2; on-chain "prompt NFT" projects drifted into agent tooling). The durable value has moved to **provenance and licensing rights over the content, not the prompt string.**

**Proposed repositioning: from "prompt-NFT marketplace" → "AI provenance + on-chain licensing infrastructure, settled in MOC."** Concretely, Mossland can:

1. **Make MOC the settlement/royalty rail for licensed AI media** — adopting **C2PA Content Credentials** and **SynthID-style detection** so every asset carries verifiable origin.
2. **Mirror Story's proven pattern** — register a work as an on-chain IP Asset with a **programmable license** (on-chain terms linked to off-chain legal text) and automate royalty splits **in MOC** on each derivative/use.
3. **Tie provenance to Mossland's agentic stack** — the **[Agentic Orchestrator](https://github.com/MosslandOpenDevs/agentic-orchestrator)** and **[BRIDGE 2026](https://github.com/MosslandOpenDevs/bridge-2026)** generate AI media and take actions; the **"AI proposes, humans decide"** governance of **[Agora](https://github.com/MosslandOpenDevs/Agora)** / **[Algora](https://github.com/MosslandOpenDevs/Algora)** is a natural place to decide licensing terms and adjudicate provenance/derivative disputes on-chain.

This turns MOC from a *marketplace currency* into the **unit of account for verifiable, licensable, agent-generated content** — aligned with the EU AI Act's Aug 2026 labeling mandate that creates real demand for compliant provenance rails.

> ⚠️ **Honest framing.** This is a *proposed* pivot. Whether MOC-denominated on-chain licensing has real demand versus incumbent rails (Story's IP token, fiat marketplaces) is unproven — a business-model risk, not a settled fact.

---

## 3. Revised 2026 research directions

1. **C2PA + SynthID reference pipeline:** attach Content Credentials to Mossland/agent-generated media at creation, verify on ingest, and expose an "inspect provenance" view — treating EU AI Act Article 50 (in force 2 Aug 2026) machine-readable marking as a compliance target, not an afterthought.
2. **On-chain IP-licensing module with MOC settlement:** register works as IP Assets, encode a programmable license (Story PIL-style on-chain terms bound to off-chain legal text), and auto-split royalties in MOC to creators and upstream sources on each licensed use/derivative.
3. **Agent-content IP policy:** since prompts / pure AI output are not copyrightable (US Copyright Office, Jan 2025), define how **human contribution, provenance, and license grants** — not the prompt — establish who may use/monetize agent-generated assets, with disputes routed through Agora/Algora governance.
4. **Provenance-and-consent registry for AI training:** let creators publish machine-readable "do-not-train / licensed-to-train" signals (à la Adobe Content Authenticity preferences) recorded on-chain, priced and licensed in MOC.
5. **"IPFi" primitives for MOC-denominated IP:** fractionalization, licensing-revenue-backed collateral, and royalty streaming for on-chain IP Assets — learning from Story's IPFi framing while scoping legal/regulatory limits.
6. **Interoperability over enclosure:** evaluate bridging with Story Protocol and C2PA verification providers so Mossland assets carry *portable* provenance and licenses across ecosystems, and benchmark watermark robustness (SynthID) against metadata-stripping attacks.

---

## 4. Open Questions & Caveats

- **"Duckee"** (a Korean AI-prompt/blockchain marketplace referenced in the original repo) **could not be verified** from authoritative sources in this review — its current existence/status is unconfirmed.
- **C2PA v2.2** exact release date and feature scope were found only via secondary sources; confirm against the official C2PA changelog.
- **Story mainnet** exact launch date (reported ~Feb 13, 2025) and network naming come from crypto press; confirm against primary sources.
- **NFPrompt's** 2025 pivot specifics come largely from project self-reporting.
- **Device-level C2PA claims** (Galaxy S25 native-camera signing, Pixel 10 chip-level C2PA) are from tech press; confirm against OEM release notes.
- The **EU Code of Practice** date/scope are from legal commentary; it is guidance, not binding law.
- **Whether MOC-denominated on-chain licensing has real demand** is unproven — a business-model risk.

---

## References

- C2PA — OpenAI joins Steering Committee: https://c2pa.org/openai-joins-c2pa-steering-committee/
- Adobe — Content Authenticity public beta: https://blog.adobe.com/en/publish/2025/04/24/adobe-content-authenticity-now-public-beta-helps-creators-secure-attribution
- Google — SynthID Detector: https://blog.google/innovation-and-ai/products/google-synthid-ai-content-detector/
- Content Credentials (overview): https://en.wikipedia.org/wiki/Content_Credentials
- Google Pixel 10 adds C2PA (context): https://android.gadgethacks.com/news/google-pixel-10-adds-c2pa-support-to-fight-ai-fakes/
- EU AI Act — Article 50: https://artificialintelligenceact.eu/article/50/
- European Commission — Code of Practice on Transparency of AI-Generated Content: https://digital-strategy.ec.europa.eu/en/policies/code-practice-ai-generated-content
- Story — Series B (TechCrunch): https://techcrunch.com/2024/08/21/story-raises-83m-at-a-2-25b-valuation-to-build-a-blockchain-for-the-business-of-content-ip-in-the-age-of-ai/
- Story — mainnet + IP token (Decrypt): https://decrypt.co/305730/story-protocol-debuts-mainnet-with-1-billion-ip-tokens-to-claim
- US Copyright Office — Copyright and AI, Part 2 (PDF): https://www.copyright.gov/ai/Copyright-and-Artificial-Intelligence-Part-2-Copyrightability-Report.pdf
- PromptBase (Tracxn): https://tracxn.com/d/companies/promptbase/__rwbBOyb3nk-QxJtJohphuSVEPTVAhLhUecHdSV8wFQ4
- NFPrompt (CoinMarketCap): https://coinmarketcap.com/currencies/nfprompt/

*This is a research/strategy note, not legal or financial advice. Contributions and corrections welcome at [contact@moss.land](mailto:contact@moss.land).*
