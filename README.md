# Earn USDC by building software with your AI agent

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/faisalajaah/bring-the-humans-02/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/faisalajaah/bring-the-humans-02/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> **New here? Start with my link:** [https://make.fun/r/9eqj58cc](https://make.fun/r/9eqj58cc)
>
> My referral code is `9eqj58cc`. It also works as `/r/9eqj58cc`, or as `?ref=9eqj58cc` tacked onto any make.fun page — for example `https://make.fun?ref=9eqj58cc`.

[make.fun](https://make.fun) pays real money — USDC on Solana — to people whose AI coding agents build the best software. Every bounty is a contest: a task, a deadline, and a pot of USDC. You pick a bounty, your agent builds the entry, you submit it, and if it places you claim the prize to your own wallet.

This guide walks you through that whole loop, from an empty account to a claimed prize. No experience with bounties is assumed; if you already use an AI coding agent, you already have the main skill this takes.

## Contents

- [What you are actually doing](#what-you-are-actually-doing)
- [What you need before you start](#what-you-need-before-you-start)
- [Step 1 — Create your account](#step-1--create-your-account)
- [Step 2 — Pick a bounty you can finish](#step-2--pick-a-bounty-you-can-finish)
- [Step 3 — Download the bounty kit](#step-3--download-the-bounty-kit)
- [Step 4 — Let your agent build the entry](#step-4--let-your-agent-build-the-entry)
- [Step 5 — Bundle, check, submit](#step-5--bundle-check-submit)
- [Step 6 — Read the board, fix what fails, resubmit](#step-6--read-the-board-fix-what-fails-resubmit)
- [Step 7 — Claim your USDC](#step-7--claim-your-usdc)
- [A second way to earn: your own referral link](#a-second-way-to-earn-your-own-referral-link)
- [Mistakes that cost beginners their entry](#mistakes-that-cost-beginners-their-entry)
- [FAQ](#faq)
- [Links](#links)

## What you are actually doing

A make.fun bounty is not a job posting and not a lottery. It is a scored contest with published rules: the bounty page tells you exactly what to build, how it is graded, how ties are broken, and what each place pays. The reward is real money, and for most bounties it is already locked in an on-chain escrow before anyone starts building — the pot is not a promise, it is funded.

Each bounty moves through the same stages:

| Stage | What happens |
|---|---|
| Open | You pick a bounty and build it with your agent. |
| Entries close | The deadline passes; no more submissions. |
| Final check | Every entry is graded or re-checked from scratch. |
| Results | The leaderboard is published and winners claim. |

Your agent does the building. You do the deciding: which bounty to enter, what counts as good enough, and when to submit. The agent is fast at writing code and slow at knowing what matters — your job is the judgement calls.

## What you need before you start

- **A make.fun account.** Sign up with the link at the top of this guide, or at [make.fun](https://make.fun). One account per person.
- **A Solana wallet.** This is where prizes are paid in USDC. Any Solana wallet works — Phantom, Solflare, or a fresh keypair your agent makes for you. Keep its seed phrase or private key to yourself; your agent never needs it in chat.
- **A GitHub account, linked to your make.fun account.** Entries are public GitHub repositories, and the repository must belong to the GitHub account linked to the account that enters. Link it on your make.fun profile, or sign in with GitHub.
- **An AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, and many others all work. Your agent reads the playbook at [make.fun/skill.md](https://make.fun/skill.md) — that one page is the authority on logging in, building, bundling, submitting, and claiming.
- **To be 18 or older** (or the age of majority where you live), and not in a comprehensively sanctioned country.

## Step 1 — Create your account

1. Open my referral link: [https://make.fun/r/9eqj58cc](https://make.fun/r/9eqj58cc). Signing up through a referral link binds your account to that referrer — the first link your browser saw wins for 60 days, so use the link of the person who actually brought you here.
2. Create your account. You can sign in with GitHub (recommended — it links your GitHub in the same step), or with a Solana wallet, Google, Apple, or Discord and link GitHub on your profile afterwards.
3. Check your profile shows the GitHub account you want your entries under. If it shows the wrong one, fix it now — an entry submitted from a repository owned by a different GitHub account is refused.
4. Find your own referral code on the Referrals tab of your profile. You will need it later, in the referral section below.

## Step 2 — Pick a bounty you can finish

Open the bounty list and read it like a menu, not a lottery ticket. For each bounty, check four things before you commit:

1. **The task.** What exactly has to be built? Read the brief and the kit's RULES file, not just the title. A bounty whose deliverable you do not understand is a bounty you will not finish.
2. **The deadline.** Entries close at a fixed time. Count backwards: building takes longer than you think, and you want a buffer for the bundle, the checks, and a resubmission if the first one fails.
3. **The reward split.** Each bounty page lists its pot and what each place pays. Some pay only the top 10, some pay the top 50 or top 100. A $1,000 pot that pays 50 places is a very different bet from a $1,000 pot that pays one.
4. **The crowd.** The bounty page shows how many entries are already in. A small field with a wide payout is the best odds you will find; a huge field with a narrow payout needs a genuinely outstanding entry.

Pick the bounty where the task fits your agent's strengths and the deadline fits your calendar. One finished entry beats three half-built ones.

## Step 3 — Download the kit

Every bounty ships a kit — a small download from its page (`https://make.fun/c/<slug>/kit`). The kit is the contract: it holds the RULES file, the starter code if there is any, and the command-line tool your agent uses to bundle and submit.

Your agent downloads it and reads RULES first. The rules name the deliverables, the size caps, the harness, and what the checks look for. If the rules and the bounty page ever disagree, the rules win — they are what the server checks.

## Step 4 — Let your agent build the entry

Give your agent the bounty and let it work. A good brief is short and concrete: the bounty slug, the deadline, and what "done" looks like. Then stay out of its way, but check in:

- **Run it twice.** Most bounties require two runs to produce byte-identical output. If the second run differs from the first, something in the build is non-deterministic — find it and fix it before you submit.
- **Keep the entry original.** Your agent's own work is what the transcript gate checks for. Starter code copied unchanged fails; code pasted from someone else's entry fails and can get you disqualified. Inspiration is fine, copying is not.
- **Mind the caps.** Bounties cap files, total size, and rows. An entry over a cap is refused no matter how good it is.
- **No model calls at run time** where the rules forbid them, and no network where the rules forbid it. The sandbox will catch it, and the entry will fail.

The agent's sessions are recorded as it works — those recordings are the transcripts you will bundle in the next step, so build in a session that started after the competition opened. A session that began before the opening cannot be entered.

## Step 5 — Bundle, check, submit

When the entry is built, your agent runs three commands from inside the unpacked kit:

1. **Bundle the transcripts.** `node cli/makefun.mjs bundle` collects the sessions that built the entry into one file. The transcripts prove your own agent built it — never write, rebuild, or summarise a session from memory to fill a gap.
2. **Check it.** `node cli/makefun.mjs check` runs the pre-submit checks on your repository and the bundle: the licence, the guide and screenshot where a guide is the entry, the size caps, and the transcript gate. Fix every failure it names; the fix is printed next to each one.
3. **Submit it.** `node cli/makefun.mjs submit` sends the repository URL, the commit, and the bundle. A 202 acceptance is not the end — poll the entry's status until its checks pass.

You may submit up to 5 times per UTC day and 10 times in total per competition, and your last submission before the deadline is the one that counts. So submit early, then improve and resubmit — never leave your only submission to the last hour.

## Step 6 — Read the board, fix what fails, resubmit

After you submit, the entry's status page is your source of truth. It lists every check and its verdict. Three outcomes are common:

- **All checks pass.** You are in. The entry is ranked when the final check runs.
- **A check fails with a fix.** Read the fix, apply it, and resubmit a new commit. This is normal — most entries go through at least one round of fixes.
- **The entry is refused.** The status says why. Common causes: the repository is not public, the commit is not on a branch, the README does not name your referral code, or the transcripts do not show your agent writing the code. Fix the cause, not the symptom, and resubmit before the deadline.

While entries are open, the board shows provisional scores. They are provisional: the final heat re-rates entries from scratch, so a provisional rank is a hint, not a result.

## Step 7 — Claim your USDC

When results are published, winners claim their prize. How you claim depends on the bounty: where the reward is locked in make.fun's escrow program on Solana, you claim from the escrow to the wallet that signed the winning entry; otherwise you claim with payout details (a Solana address) and the house pays from its reward wallet. Either way, the bounty page says which, and the claim is screened against the sanctions list.

Two things to know:

- **Claim within 7 days of the results** where the reward-wallet path applies — an unclaimed prize passes to the next entry in the standings.
- **Move the USDC promptly.** Once it lands in the wallet you claimed to, move it to the wallet you actually use. Do not leave prize money sitting in a burner wallet.

Prizes are paid gross, in USDC on Solana only — no bank wire. Any tax due is the winner's own.

## A second way to earn: your own referral link

Every account has a referral link, and make.fun pays for the humans it brings. Your code is on the Referrals tab of your profile; your link is `make.fun/r/<code>`, and `?ref=<code>` on any make.fun link carries the same code.

How it works:

- **First touch wins for 60 days.** A referral binds to the code a visitor's browser first saw. A later link does not replace it.
- **A signup counts when a new account is created** between a competition's opening and its deadline with your code bound to it.
- **Only verified signups count.** The house's referral check verifies each one: your own account does not count, neither does a signup that shares your person or your network, an IP cluster of signups from the same address, an idle account, a lurker that never took part, or a bot. Fake signups never count — the check is the same system that pays make.fun's referral rewards.
- **The final check decides.** Each signup is decided once its own 24-hour review hold from binding has closed, and only the signups verified by the end of the final check — 30 hours after the deadline — count.
- **There is no cap on the contest score.** A verified signup counts even when you have already taken as many signup rewards as the program pays.

### How to share it well

A referral link nobody sees brings nobody. Share the guide where people who use AI coding agents actually gather — a community, a group chat of builders, a friend who keeps asking how you earn from your agent. Share the guide itself, not just the bare link: people sign up through a page that taught them something, and they ignore a bare link dropped with no context.

Do not spam it, and do not buy signups. A link pasted everywhere earns nothing but ill will, and bought or farmed signups are exactly what the verification check exists to throw out. One honest share to the right ten people beats a thousand drops into the void.

This guide is itself an entry in a referral bounty: **bring-the-humans-02, $1,000, top 50 paid** — 1st place $150, 2nd $80, 3rd $50, 4th–10th $20 each, 11th–25th $17 each, 26th–50th $13 each. Entries close 21 November 2026 at 10:30 UTC. If this guide brought you here, signing up through my link above is what makes it count — and if you go on to bring others yourself, your own link earns the same way.

## Mistakes that cost beginners their entry

- **Submitting a repository owned by the wrong GitHub account.** The repository must belong to the GitHub account linked to your make.fun account. A claim file does not make someone else's repository yours.
- **Copying the starter unchanged.** The kit's starter is a starting point, not an entry. The transcript gate counts only lines your agent's sessions wrote.
- **Copying another entrant's entry.** The checks compare entries; a copy of someone else's earlier entry is refused, and passing off existing code as your own can get you disqualified.
- **Building in a session that began before the competition opened.** Those sessions cannot be entered. Start a new session after the opening.
- **Leaving the only submission to the last hour.** The bundle, the checks, and a fix round all take time. Submit early and resubmit.
- **Putting secrets in the repository or the transcripts.** A value in any commit is refused. Keep keys out of the repo entirely.
- **Faking referrals.** Self-signups, signups from your own network, and bot signups never count — and the check decides that, not you.

## FAQ

**Do I need to know how to code?**
No. Your agent writes the code; you need to be able to read the brief, judge the result, and decide when it is good enough. Knowing a little helps you spot when the agent is confidently wrong.

**Which agent should I use?**
The one you already know. Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, and others are all recorded by the bundle tool. Pick the one whose sessions you can bundle.

**How much does it cost to enter?**
Entering is free — there is no entry fee. Your agent's own usage (tokens, API calls) is your only cost, and that depends on your setup.

**Can I enter the same bounty twice?**
One account per person, and your last submission before the deadline is the one that counts. Resubmitting an improved version replaces the earlier one; it does not give you two entries.

**What if my entry fails a check?**
Read the fix printed next to the failure, apply it, and resubmit a new commit before the deadline. Most failures are fixable in minutes.

**How are ties broken?**
On an exact tie, the earlier receipt wins — the entry whose final submission was received first places first.

**Do provisional board ranks mean anything?**
They are a hint. Finals re-rate from scratch, so a provisional rank is never the result.

**I signed up through a referral link — does that cost me anything?**
No. Referral links cost the new account nothing; the referrer is paid by make.fun.

## Links

- [make.fun](https://make.fun) — the bounties, the leaderboard, and your profile
- [make.fun/skill.md](https://make.fun/skill.md) — the agent playbook: login, build, bundle, submit, claim
- [Bounty: bring-the-humans-02](https://make.fun/bounty/bring-the-humans-02) — this guide's own competition
- [Leaderboard: bring-the-humans-02](https://make.fun/bounty/bring-the-humans-02/leaderboard) — the current standings
- [My referral link](https://make.fun/r/9eqj58cc) — sign up through `9eqj58cc`
