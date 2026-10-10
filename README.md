# grind 75 vs blind 75: which list to actually finish, how long each one takes, and where to learn the patterns behind both

Most people asking about Grind 75 vs Blind 75 are not really choosing between two lists. They are trying to answer three questions at once: how many problems do I need to solve, in what order, and what do I do when I get stuck on problem 12 and the list offers no help.

Those questions have answers. They are just scattered across a redirect page, a GitHub repo, and a dozen blog posts that copy each other.

Here is the short version, then the details.

**Blind 75** is a fixed set of 75 problems, grouped by topic, published in 2018. **Grind 75** is its replacement, written by the same person in 2022, and it works differently: it ranks a pool of 169 problems and hands you the top 75 as a schedule you can stretch or compress based on the hours you actually have.

Both are free. Both are good. Neither teaches you anything.

## What actually changed between the two lists

Both lists come from Yangshun Tay, a former Meta staff engineer who also wrote the Tech Interview Handbook. That detail matters more than it sounds, because Grind 75 is not a competitor's attempt to improve on Blind 75. It is the original author saying his own list had structural problems.

His complaint, in his own words, was that "the Blind 75 list is static, non-personalized and questions do not have a priority." Notice what is not in that sentence: he never says the problems were badly chosen. He says 75 turned out to be too few for a lot of people, and that a flat list cannot know whether you have three weeks or three months.

|  | Blind 75 | Grind 75 |
| --- | --- | --- |
| Published | 2018, posted on the Blind app | 2022, by the same author |
| Size | Fixed at 75 problems | Ranked pool of 169, default plan uses the top 75 |
| Ordering | Grouped by topic | Ordered by difficulty, topics interleaved across weeks |
| Difficulty mix | About 19 Easy, 49 Medium, 7 Hard | 24 Easy, 42 Medium, 9 Hard in the default 75 |
| Time controls | None | You set available weeks and hours per week |
| Premium problems | Mixed in | Pushed to the end; none in the first 75 |
| Where it lives now | Dropped from its own domain; grind75.com redirects into the Tech Interview Handbook | Same page, actively maintained |
| Cost | Free | Free |

Two of those rows deserve a closer look.

The first is ordering. Blind 75 groups everything by topic, so you do nine array problems, then fourteen tree problems, then the graph block. It feels tidy. It is also a weaker way to learn, because after your fifth consecutive binary tree question you stop reading the problem and start pattern-matching on the section header. In a real interview nobody tells you the category. Grind 75's answer is to mix topics within each week so you have to identify the pattern yourself, repeatedly, instead of once per block.

The second is the premium filter. Grind 75 deliberately keeps LeetCode Premium-only questions out of the initial 75 and pushes them as far back as possible. If you are not paying for LeetCode Premium, that single design decision affects your study week more than any sorting detail.

## The 169 problems did not come from nowhere

Grind 75's FAQ explains the construction, which is unusually transparent for a prep product. The starting pool came from Blind 75 itself, Sean Prashad's LeetCode Patterns collection, questions from Elements of Programming Interviews, and a few other pattern lists. The author then sorted LeetCode by popularity, frequency, company tags, likes and topic coverage, looked at the top 200 in each dimension, and added anything that was missing. Problems got tagged by pattern, ranked inside that pattern, and then flattened into one ordered list that gets sliced into weeks.

Two ranking rules came out of that process:

- Easy problems go first. The reasoning is that an easy problem teaches a pattern you will reuse later, so it is worth the early slot.
- Hard problems get pushed down. The stated reason is that hards usually run past thirty minutes, while the most common difficulty in an actual coding interview is Medium. The result is a default list that is more than half Medium.

There is also a blunt piece of advice on the Tech Interview Handbook from the same author, aimed at what to skip rather than what to add: the return on investment from grinding dynamic programming questions is, in his assessment, low. Plenty of people ignore that and grind DP anyway.

## Which one to pick, based on how much time you have

The honest answer depends on your calendar, not on which list is newer.

**Two weeks or less.** Use Grind 75's time controls to generate a small subset instead of attempting all 75. If your interview is that close, working through 75 new problems produces shallow recognition, not skill. Blind 75 works better here as a checklist if you have already seen many of its problems and just need to find the holes.

**Three to six weeks.** Grind 75. The priority ordering is worth something specific: if a busy week cuts your study time in half, you lose the bottom of the list rather than a random chunk of it. Keep the interleaved topic order instead of resorting the problems by topic. The discomfort of switching patterns is the point.

**Eight to twelve weeks.** Grind 75 again, and there is no need to expand all the way to 169 problems just because the pool exists. Expand only when your error log shows a specific topic that needs more examples.

**Already strong, just maintaining.** Blind 75's compactness works in your favor. Skip anything you can solve cleanly on the first read and spend the time on patterns that have decayed.

One more thing worth saying plainly: finishing a list is not the same as owning it. A row of checkmarks does not mean you can handle a problem you have never seen, and that is the only thing the interview actually tests.

## Where both lists stop helping

Blind 75 and Grind 75 have the same structural limitation, and it is not the problem count.

They are lists. They tell you what to solve and in what order. They do not explain why a solution works, they do not tell you which pattern a new problem belongs to, and they do not tell you where your reasoning broke when your code fails. That gap is exactly where a lot of people stall around problem 20: they can read a solution, but they cannot produce the next one unaided.

That is the gap pattern-based courses are built for, and it is why you see so many people running a list and a course at the same time rather than picking one. A user on Blind described the division of labor well: AlgoMonster is "more like taking a class that explains all of the patterns" while Grind 75 is "just doing the LC themselves for reps with no explanation."

[👉 See how AlgoMonster structures its pattern lessons and practice lists](https://algo.monster?fpr=li69)

## What AlgoMonster adds to either list

AlgoMonster is a pattern-based interview prep platform built by former Google engineers. It is text and diagram based, not video based, and it is organized around roughly 48 coding patterns rather than around a problem count.

The part that connects directly to this comparison: AlgoMonster's practice area includes its own curated lists, and one of them is Blind 75. The version on their site runs 73 problems, each mapped to the patterns taught in the curriculum, so a problem is not just a name in a table. You get the pattern, a template, and feedback on where your approach went wrong. There is also a shorter 50-problem list for people who want a tighter scope.

Other pieces that matter in practice:

- **Speedrun mode** for timed review, which is the closest thing on the platform to interview pressure.
- **An AI assistant** for hints and code analysis when you are stuck, so you are not stuck for an hour.
- **Pattern decision flowcharts** — the "is the input sorted, am I looking for a contiguous range" style questions that get you to the right approach before you write code.
- **Company-oriented question sets**, updated monthly, alongside the pattern curriculum.
- **Bonus courses included with a subscription**: a CS foundation course and a "build an LLM" course. Some specialized content, such as the quant interview prep course, is sold separately.

Reviewers are consistent about the tradeoffs too. The platform is entirely text and interactive diagrams, so if you learn by watching someone code, this format will feel dry. The problem bank is in the low hundreds rather than the thousands, so most people still use LeetCode for volume. System design coverage is introductory, and there are no live mock interviews with real engineers. If you are targeting L5 or above, plan on a separate system design resource.

## AlgoMonster plans and current pricing

There is no monthly plan. The choice is free, annual, or lifetime, and the paid prices shown at checkout are currently about half of what deal blogs list as the original price.

| Plan | What you get | Price | Billing | Get started |
| --- | --- | --- | --- | --- |
| Free | Limited sample content, plus access to the practice tab and curated lists | $0 | — | [ Open the free practice lists](https://algo.monster?fpr=li69) |
| Pro — Yearly | All patterns, lessons and problems; AI assistant; Speedrun; company question sets; bonus foundation and LLM courses | $99 (about $8.25/month) | Billed annually; the page currently advertises a 3-day trial before the annual charge | [ Check the yearly plan](https://algo.monster?fpr=li69) |
| Pro — Lifetime | Everything in the annual plan, plus lifetime updates and an internal referral to a top tech company for qualified candidates | $189 | One-time payment | [ See the lifetime plan](https://algo.monster?fpr=li69) |

Two cautions, both worth checking before you pay.

Pricing on this site moves. Older third-party writeups quote anything from $119 to $459 for a year and $459 for lifetime, while the current checkout page shows $99 and $189. Sales are frequent and the discount is applied automatically, so the number you see on the page is the only one that means anything.

Also, several review sites describe AlgoMonster as offering a job guarantee. The wording on the pricing page is narrower than that: lifetime access includes an internal referral to a top tech company for qualified candidates. Treat "referral for qualified candidates" and "guaranteed job offer" as different promises.

## How to combine the two without wasting weeks

The order that wastes the least time, based on how these tools are actually designed:

1. Learn the patterns first, a few problems each, with something that explains the why. This is the phase a problem list cannot cover, because a list has no explanation layer.
2. Run Grind 75 (or Blind 75 if you are short on time or reviewing) as your practice volume, alongside LeetCode when you need more reps on a specific topic.
3. Keep an error log. Expand past the default 75 only when that log names a topic, not because the pool contains 169 problems.
4. In the last third of your available time, switch to company-specific questions and timed practice rather than more new patterns.

If you are starting today with no particular deadline, Grind 75 plus a pattern course is a better use of six weeks than either one alone. If you already know the patterns and your problem is speed and volume, skip the course, keep Blind 75 as a checklist, and grind real company questions.

The list was never the hard part. Recognizing the pattern in a problem you have never seen is, and that is the part no list does for you.

[👉 Start with the free practice tab and see if the pattern approach fits how you learn](https://algo.monster?fpr=li69)
