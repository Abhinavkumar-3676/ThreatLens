# ThreatLens 🛡️ — Digital Risk Protection & Brand Defense Platform

An enterprise, explainable, and audit-compliant **Digital Risk Protection (DRP)** platform specializing in **Social Media Impersonation Defense** and **Mobile App Store Monitoring**, anchored by a verified multi-channel **Brand Baseline Exclusion Engine** that guarantees zero false positives for registered corporate assets.

---

## 🚀 Quick Start

The platform is running locally at:
👉 **[http://localhost:3000](http://localhost:3000)**

### Running the Development Server
```bash
# In the threatlens directory
pnpm run dev
# Starts Next.js with hot reloading at http://localhost:3000
```

### Database Seeding & Reset
```bash
# Seed or reset the SQLite database with rich threat fixtures
pnpm exec tsx prisma/seed.ts
```

---

## 🏆 Hackathon Alignment & Weighted Feature Architecture

| Category | Weight | ThreatLens Capability | Implementation Details |
| :--- | :---: | :--- | :--- |
| **Social Media Monitoring** | **30%** | **Cross-Platform Impersonation Detection** | Flags rogue customer support bots, executive (VIP) impersonation, counterfeit promotional airdrop phishing, and bio credential harvesting across **X/Twitter, LinkedIn, Instagram, and Telegram**. |
| **App Store Monitoring** | **30%** | **Mobile Ecosystem Defense** | Detects package identifier namespace squatting (`com.threatlens.*`), publisher verification mismatches, trojanized utility modifiers ("Helper", "Plus", "Mod"), and predatory permissions (SMS interception, accessibility service). |
| **Brand Profile Baseline** | **15%** | **Multi-Channel Exclusion Engine (0 False Positives)** | Registers corporate domains, social handles, mobile package bundle IDs, and VIP rosters. Systematically bypasses threat scoring with guaranteed **0 / 100 risk** for verified assets before evaluation. |
| **User Experience & SOC Triage** | **15%** | **Enterprise Cyber Dark Console & Case Vault** | Obsidian glassmorphism UI, real-time telemetry feed, case lifecycle triage (Under Review, Confirmed, Resolved), Evidence Locker with **cryptographic SHA-256 hashes**, analyst notes timeline, and immutable audit logging. |
| **Presentation & Evaluator Demo** | **10%** | **1-Click Judge Demo Scenarios & Audit Export** | Instant interactive evaluation launcher for hackathon evaluators to test VIP social mimicry, rogue Android packages, and baseline exclusions with explainable heuristic math. 1-click formatted JSON compliance audit export. |

---

## 🧩 Architectural Overview

```text
threatlens/
├── prisma/
│   ├── schema.prisma        # Complete SQLite / Postgres schema (User, Brand, OfficialAsset, Finding, Investigation, Evidence, AuditLog)
│   ├── dev.db               # SQLite active operational database
│   └── seed.ts              # Full deterministic seed data
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   ├── analyze/     # Live explainable heuristic scoring engine endpoint
│   │   │   ├── brand/       # Multi-channel baseline asset CRUD
│   │   │   ├── export/      # Formatted NIST / SOC2 JSON compliance export
│   │   │   ├── findings/    # Incident candidate retrieval & status transitions
│   │   │   ├── investigations/ # SOC case management & analyst notes
│   │   │   └── reset/       # 1-click database reset for judges
│   │   ├── globals.css      # Obsidian theme, glassmorphism panels, glowing cyber accents
│   │   ├── layout.tsx       # Root layout & meta tags
│   │   └── page.tsx         # Unified SOC dashboard orchestrating all views
│   ├── components/
│   │   ├── Navbar.tsx             # Header, radar pulse, 1-click scenarios launcher, export button
│   │   ├── OverviewTab.tsx        # Command Center KPI metrics & live threat telemetry feed
│   │   ├── SocialMediaTab.tsx     # 30% Category: X, LinkedIn, Instagram, Telegram impersonation cards
│   │   ├── AppStoreTab.tsx        # 30% Category: Google Play, App Store, APK Mirror defense
│   │   ├── DomainTab.tsx          # Lookalikes, Levenshtein distance, homoglyphs (threatl3ns.io)
│   │   ├── InvestigationsTab.tsx  # SOC Cases, triage workflow, evidence vault
│   │   ├── BrandProfileTab.tsx    # 15% Category: Multi-channel baseline asset manager
│   │   ├── QuickScannerTab.tsx    # Interactive scanner with real-time heuristic signal math
│   │   ├── JudgeScenariosModal.tsx # 10% Category: 1-Click judge evaluation scenarios
│   │   ├── CaseDetailModal.tsx    # Evidence locker, SHA-256 hashes, analyst notes composer
│   │   └── AddAssetModal.tsx      # Add official assets directly into baseline
│   └── lib/
│       ├── db.ts            # Prisma client singleton
│       └── heuristics.ts    # Pure, deterministic, offline heuristic scoring & exclusion engine
```

---

## 🔬 Explainable Heuristic Signal Rules & Math

### 1. Multi-Channel Baseline Exclusion Engine
- Checks input against registered official domains, social handles, and app package bundle IDs.
- If an exact normalized match exists:
  - **Risk Score**: `0 / 100` (Zero False Positive Guarantee)
  - **Status**: `Protected Official Asset`
  - **Notice**: *"EXCLUDED BEFORE THREAT SCORING: Exact match with registered official asset"*

### 2. Social Media Heuristics (30% Weight)
- Monitored brand stem in handle: `+25`
- Customer support lure tokens (*support, help, desk, bot, care*): `+30`
- Promotional incentive cues (*airdrop, rewards, bonus, giveaway*): `+25`
- VIP executive persona match against monitored leadership roster: `+30`
- Authority modifier suffixes (*_official, _bot, _team*): `+15`
- Bio credential harvesting / private key solicitation cues: `+25`
- Off-platform shortened redirects (*bit.ly, linktr.ee*): `+15`

### 3. App Store Heuristics (30% Weight)
- Package namespace squatting (`com.threatlens.*`): `+30`
- Trojanized utility descriptors (*Helper, Plus, Mod, Pro, Tool*): `+25`
- Publisher entity mismatch against verified corporate entity: `+20`
- Non-store sideloaded mirror format (APK mirror / unregulated signing): `+20`
- Predatory permission vectors (*SMS interception, accessibility service binding*): `+18`

### 4. Domain & Web Host Heuristics
- Monitored corporate brand keyword in root label: `+20`
- Authentication & SSO phishing lure tokens (*login, secure, verify, auth, portal*): `+25`
- Deceptive multi-hyphenation (&ge; 2 hyphens): `+15`
- Homoglyph leetspeak character substitutions (e.g. `3` &rarr; `e`): `+35`
- Low Levenshtein edit distance (&le; 2) against primary authoritative domain: `+25`
- Adjacent character transpositions (Damerau-Levenshtein swaps): `+30`

---

## 🧪 Testing Checklist for Evaluators

1. **Launch Console**: Open `http://localhost:3000`.
2. **Review Metrics**: Inspect KPI cards on the **Command Center** showing real active candidate counts and baseline exclusions.
3. **Judge 1-Click Scenarios**:
   - Click **Judge 1-Click Scenarios** in the top navigation bar.
   - Click **Launch Scenario** on *Scenario A (VIP Executive Impersonation)* or *Scenario B (Trojanized 2FA APK)*.
   - The scanner evaluates the candidate and displays the exact signal weights and risk scores.
4. **Test Baseline Exclusion Safeguard**:
   - In the **Quick Threat Scanner**, enter `threatlens.io` with category `Domain Host`.
   - Click **Analyze Threat Risk**.
   - Notice the score locks at **0 / 100** with the green badge: *"EXCLUDED BEFORE THREAT SCORING: Exact match with registered official corporate domain"*.
5. **Inspect SOC Cases**:
   - Navigate to the **SOC Investigations** tab.
   - Click on case **TL-2026-081** or **TL-2026-082**.
   - Review attached findings, cryptographic SHA-256 evidence hashes, and post a new analyst note in real time.
6. **Download Compliance Audit**:
   - Click **Export Audit** in the top navigation bar to download the formatted JSON audit trail.
