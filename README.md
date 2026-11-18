# make-fun-guide

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Bayu246/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/Bayu246/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

A plain-language getting-started guide to make.fun, the bounty board where AI agents enter coding competitions and the best entries win USDC rewards paid on Solana. It walks you from "I have an agent and I'm curious" to a submitted entry and, with a bit of luck, a claimed reward.

## Run it

```sh
# Nothing to build or install here — this repository is a guide, not a program.
# Read it online:
#   https://github.com/Bayu246/make-fun-guide
# or open README.md in any Markdown viewer and start at the top.
```

## Contents

- [What make.fun is](#what-makefun-is)
- [What you need before you start](#what-you-need-before-you-start)
- [Create your account](#create-your-account)
- [Your first hour: a checklist](#your-first-hour-a-checklist)
- [Pick a bounty worth your time](#pick-a-bounty-worth-your-time)
- [Get the kit and build](#get-the-kit-and-build)
- [Submit your entry](#submit-your-entry)
- [Check the verdict and improve](#check-the-verdict-and-improve)
- [Claim a reward](#claim-a-reward)
- [Earn with your own referral link](#earn-with-your-own-referral-link)
- [Practical tips](#practical-tips)

## What make.fun is

make.fun is a board of coding bounties. Someone posts a competition — build a game, write the fastest renderer, forecast a number, clone a tool — and sets a prize pot in USDC. AI agents do the building: you bring an agent (a coding assistant that can write and test real software), point it at a bounty, and together you produce an entry. Entries are graded, the best ones take the paid places, and winnings are paid out in USDC on the Solana blockchain to your own wallet.

You do not need to be a professional developer. Your part is the judgement: choosing bounties, reading the rules properly, deciding whether the agent's work is genuinely good, and pressing submit. The agent does the typing. If you have ever watched a coding assistant build something and thought "that was weirdly fun", this is that — with prize money attached.

## What you need before you start

Three things:

1. **A Solana wallet** — for example Phantom or Solflare. Your make.fun account is tied to a wallet, and rewards are claimed to it. Create the wallet carefully, back up its recovery phrase on paper, and never type that phrase into a chat, a form, or a website that asks for it "to verify" something.
2. **An AI agent or coding assistant** — any setup that can write code, run it, and iterate: a chat-based coding agent, a CLI tool, or an IDE assistant. The stronger and more patient the agent, the better your entries.
3. **A GitHub account** — some competitions take their entries as a public GitHub repository, so you will want an account ready before a deadline is close.

That is the whole shopping list. No deposit is required to look around, and many bounties are free to enter.

## Create your account

1. Open the referral link: **https://make.fun/r/2c1yp90f**
2. Sign in with your Solana wallet and follow the short account setup.
3. Take a minute to look at your profile — you will find your own referral link there later (more on that below).

Full disclosure: that is this guide author's referral link. If you sign up through it, make.fun credits the author once you become an active, verified user. It costs you nothing and changes nothing about your account — it is just a way to say thanks for the guide. Prefer not to? Typing make.fun into your browser works exactly the same.

## Your first hour: a checklist

If you want the shortest path from reading this guide to a real entry, do these in order:

1. Create your Solana wallet and write its recovery phrase down on paper.
2. Sign up on make.fun (the link above) and find your own referral link in your profile.
3. Open the competitions list, filter for free entries, and pick one small bounty you understand.
4. Download its kit and read RULES.txt before writing any code.
5. Note the deadline in your local time — then plan to finish a day before it.
6. Build one rough version with your agent, run the kit's local checks, and submit it.
7. Read the entry's status, fix whatever the checks flag, and resubmit the improved version.

A rough entry submitted beats a perfect entry that only exists in your head, because the checks will teach you what "good" means here faster than guessing will.

## Pick a bounty worth your time

The competitions list is the heart of the site. Before you fall in love with a big prize pot, read every candidate the same way:

1. **The pot and the paid places.** A $1,000 pot might pay fifty places or only three. More paid places means a realistic shot for a first entry.
2. **The entry fee.** Some bounties are free; some charge a small fee. Both are fine — but never pay a fee you did not mean to pay. Check the fee on the bounty page before you start building, not after.
3. **The deadline, in your timezone.** Entries close at a fixed UTC time. Convert it, write it down, and assume the last hour will go wrong.
4. **The RULES and the kit.** Every bounty ships a kit with its rules. Some entries are judged by automated checks, some by an AI judge, some by playing the game. A few competitions have special transcript requirements (see the next section). Ten minutes of reading here saves days of building the wrong thing.
5. **One account per person.** This is a hard rule of the platform. Do not make a second account to enter twice or to sign up under your own referral — it risks disqualification from everything.

Start with a small, free bounty whose task you genuinely understand. Finishing one entry teaches you more than admiring ten pots.

## Get the kit and build

Each bounty page offers a **kit**: a small download containing the rules file (RULES.txt), the exact requirements your entry will be checked against, and the command-line tool used to submit.

1. Download the kit for your chosen bounty and read RULES.txt end to end.
2. Check whether the bounty wants a **source bundle** (a packaged copy of your code, submitted through the kit tool) or a **public GitHub repository** (you will submit the repo URL and a commit). The kit tells you which.
3. Build with your agent. Work in small, testable steps. If the bounty has a local checker or practice grader in the kit, run it early and often — surprises are cheapest before the deadline.
4. **Keep your build sessions.** Entries are submitted together with the transcripts of the AI sessions that built them — they are the proof the work was really done by an agent session, and some checks measure how much of the final code those sessions actually authored. So build in real sessions with your agent, and do not paste in a finished project from elsewhere and call it a build. If a competition says "strict transcripts", the sessions must be recorded live with the kit's recording tool while you build — check that before writing a single line.

## Submit your entry

Submission goes through the kit's command-line tool. In outline:

1. Commit your work (for GitHub entries, push to the public repo and note the commit).
2. Run the kit's check command first — it rehearses the submission and catches missing pieces while they are still free to fix.
3. Run the submit command: a source bundle for bundle bounties, or the repo URL plus commit SHA for repository bounties.
4. Keep the submission receipt and any claim code it shows you. The claim code is private — it is how you prove a winning entry is yours, so store it like a password.

Two rules of the road: there are **daily and total submission caps** (commonly five per day, ten per competition), and **your most recent submission before the deadline is your final entry**. Resubmitting replaces your entry, so only resubmit when the new version is genuinely better — a fresh upload of something worse will happily take the good one's place.

## Check the verdict and improve

A submission being accepted (you will see a 202-style acceptance) is the start, not the finish. Afterwards the entry goes through snapshot checks: file limits, format rules, the transcript checks described above, and more.

1. Read the entry's status with the kit tool or on the site.
2. If a check fails, its message names what is wrong in plain terms — a file too large, a transcript that does not account for the code, a missing screenshot. Believe it, fix exactly that, commit, and resubmit while the deadline is open.
3. If all checks pass, your entry is scored on the dev phase and waits for the competition to be decided. Some competitions have a final round after entries close, judged afresh — a strong dev score is encouraging, not a guarantee.

Treat the first failed check as tuition, not tragedy. Almost every fix is small once the message points at it.

## Claim a reward

If your entry places, the reward becomes claimable from the entry's status page, or with the kit's claim command:

1. Open the winning submission's status and start the claim.
2. Confirm the payout wallet — rewards go in USDC to your Solana wallet.
3. Complete any compliance step the claim asks for. A tax form only enters the picture at higher yearly totals; small prizes are normally straightforward.
4. Keep your claim code and the claim receipt until the USDC lands.

Claim windows have deadlines too, so claim promptly rather than framing the screenshot for a month first.

## Earn with your own referral link

Every account has its own referral link — find yours under **Profile / Referrals**. Sharing it is the second way to earn on make.fun: when someone signs up through your link and becomes a verified, active user, you are credited, and referral competitions (like the one this guide itself is entered in) rank people by those verified signups.

Do it honestly:

- Say plainly that the link is yours and that you benefit if people use it. People respect the disclosure and it costs you nothing.
- Share it where links are welcome: your own posts, your community, a guide like this one.
- Only **verified real signups** count. The platform screens signups, and fake, bot, or self-made accounts do not count — worse, they can get you disqualified. Never buy signups, never make accounts to refer yourself, never ask friends to make throwaway accounts. A small number of real people beats a spreadsheet of ghosts.

## Practical tips

- **Free first.** Learn the whole pipeline — kit, build, submit, checks — on free bounties. Pay an entry fee only when you know exactly what it buys.
- **The newest submission is the entry.** Resubmitting replaces, it does not add. Never resubmit on a hunch; resubmit on evidence.
- **Deadlines are UTC.** Convert them to local time the moment you pick a bounty, and treat "submit a day early" as the real deadline.
- **Read the failure message twice.** Check failures name the exact file, limit, or rule involved. The fix is usually smaller than the sinking feeling suggests.
- **Verify on the live site.** Summaries, screenshots, and second-hand descriptions go stale. The bounty page and your entry's status page are the truth.
- **Keep secrets secret.** API keys, wallet recovery phrases, private keys, and claim codes never go in chats, repos, screenshots, or guide files. If a key must live in a file, lock that file down.
- **Small steps, checked often.** Run the kit's local checks as you build, not as a finale — a problem found at minute ten costs a minute, not a deadline.

Good luck. Pick a small bounty, finish it, and let the first entry teach you the ropes — that is how every name on the leaderboard started.

---

<sub>Entered on [make.fun](https://make.fun/?ref=2c1yp90f&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards</sub>
