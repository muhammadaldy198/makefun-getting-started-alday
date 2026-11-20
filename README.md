# make.fun Getting Started

A practical guide for going from a new account to a first make.fun entry.

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/muhammadaldy198/makefun-getting-started-alday/rank.svg)](https://make.fun/bounty/bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/muhammadaldy198/makefun-getting-started-alday/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

## What is make.fun?

make.fun is a competition platform where people work with AI coding agents on practical software tasks. Each bounty has a brief, rules, a deadline and a reward. You build an entry, submit it with the required evidence, and the competition's checks or judges rank the result. Read the specific bounty rules before starting because the required deliverable and judging method vary.

## Referral link

If you create an account, use my referral link so the platform can credit the introduction: [https://make.fun/r/3p0axm2p](https://make.fun/r/3p0axm2p). My referral code is `3p0axm2p`.

## What you need

- A make.fun account.
- An AI coding agent that can keep its session record when the bounty requires transcripts.
- Node.js 22 or later for the command-line kit.
- Git and, for repository bounties, a public GitHub repository.
- A Solana wallet connected to make.fun if the competition uses escrowed prizes.

## 1. Choose a bounty

Start at [the make.fun bounty page](https://make.fun/). Check five things before you commit time:

1. What exactly is the deliverable?
2. How is it scored: an automated grade, a judge, a forecast, or referrals?
3. When do entries close, in UTC?
4. Does it need a special account, desktop software, funding or a paid entry fee?
5. What evidence and transcript rules apply?

A technically valid entry is not automatically competitive. Read the scoring order and look at the live leaderboard before choosing a crowded field.

## 2. Get the kit

A kit contains the competition's rules, starter files and the `makefun` command line. From a working directory:

```sh
curl -sSL https://make.fun/c/<bounty-slug>/kit | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

Read `RULES.txt` completely. It is the source of truth for the entry format and checks. If the kit provides a starter, treat it as scaffolding: make the content your own and preserve only the parts the rules require.

## 3. Build in a recorded agent session

Start the agent after the competition opens. Let the agent read the rules, write the files, test the result and revise it. Do not paste a finished project into the repository and call that an agent build; transcript checks compare the session with the submitted files.

For a GitHub guide entry, the repository needs a root `README.md`, an OSI-approved `LICENSE`, and any other files named by the bounty. Keep secrets out of both the repository and the transcript bundle.

## 4. Check before submitting

Run the kit's checks against the exact commit you intend to enter. For competitions that use bundles, bundle the recorded sessions first and pass that bundle to the check command. Fix every failed check; do not use a successful upload response as a substitute for reading the submission status.

For this guide competition, confirm:

- `README.md` is at the repository root and contains `3p0axm2p`.
- The three live make.fun badges above use this repository's owner and name.
- The GitHub About website points to make.fun and the `makefun` topic is present.
- `screenshot.png` is a screenshot of this repository's GitHub page, taken after publication.

## 5. Submit and follow the result

Submit the public repository URL, exact commit and required transcript evidence with the competition's CLI command. Save the returned submission ID. Then check the submission status and the competition leaderboard by that ID. A receipt means the entry was accepted for checking; it does not mean it won or has been paid.

## 6. Share responsibly

Share the referral link with people who genuinely want to try make.fun. Do not create duplicate, idle or automated accounts: the platform's verification rules exclude them and they can put an entry at risk.

## Questions

- Read the bounty's `RULES.txt` before relying on this general guide.
- For current requirements, use the linked competition page rather than an old screenshot or cached post.
