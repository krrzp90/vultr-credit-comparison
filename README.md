# Vultr deal: $300 credit, deposit match, or 50% off your first two invoices — which one actually saves more? (current plan and GPU pricing included)

Vultr is running five new-customer offers right now: four credit codes listed on its own coupon page (**VULTRMATCH**, **FLY300VULTR**, **250VULTRFLY**, **FLYTWOHUNDRED**) and a separate promotion that halves your first two invoices. All of them require a new account, none can be combined with another offer, and the credit codes only apply to "select products." Your choice depends on how much you will spend in your first two months, so this guide covers the exact terms, current plan and GPU pricing, and when the 50% promotion beats a $300 credit.

> **Quick pick:** testing Vultr or running a short project → **FLY300VULTR** ($300 credit, the largest on the page). Expecting more than **$600** in bills across your first two invoices → the **50% off** promotion saves more. Already planning to fund the account with $100 → **VULTRMATCH** doubles it. 👉 [See the live codes on Vultr's coupon page](https://vultr.com/coupons?ref=9738262-9J)

## The four credit codes, side by side

| Code | What you get | Ceiling | Main condition |
| --- | --- | --- | --- |
| VULTRMATCH | Dollar-for-dollar match on your first deposit | $100 bonus | You must make a deposit |
| FLY300VULTR | $300 promotional credit | $300 | Select products only |
| 250VULTRFLY | $250 promotional credit | $250 | Select products only |
| FLYTWOHUNDRED | $200 promotional credit | $200 | Select products only |

**FLY300VULTR** is the code behind most "$300 Vultr" ads, and it is the biggest number on the official page. The offer asks for no matching deposit; the coupon page describes it as trying Vultr free with $300 in credit. That credit is promotional rather than cash, applies to select products, and cannot be combined with any other offer. Before planning a GPU cluster around it, note that "select products" is a real restriction, and the coupon page does not list which products qualify.

**250VULTRFLY** and **FLYTWOHUNDRED** are the same offer at smaller amounts. Unless something specific makes you ineligible for the $300 code, there is no reason to take $200 or $250 instead.

**VULTRMATCH** works differently. You deposit, and Vultr matches it up to $100. Put in $50 and you have $100 of balance; put in $100 and you have $200. Because the match is capped at $100, it is worth exactly 50% on a $100 deposit and proportionally less above that: a $400 deposit gets you $500, which is a 20% bonus. This code only makes sense if you were going to fund the account anyway, and the money you deposit stays yours to spend after the bonus credit is used.

## What the credit actually buys: current plan pricing

Vultr bills compute hourly and caps the charge at a monthly maximum, so the monthly figure below is what a continuously running instance costs you. These are the entry configurations:

| Plan family | Entry configuration | Price | Billing | Start |
| --- | --- | --- | --- | --- |
| Cloud Compute — Regular | 1 vCPU, 0.5 GB RAM | $0.0034/hr (~$2.50/mo) | Hourly, monthly cap | [Use the $300 code](https://bit.ly/VuLtr) |
| Cloud Compute — Regular | 1 vCPU, 1 GB RAM | $0.007/hr ($5/mo) | Hourly, monthly cap | [Open this tier](https://bit.ly/VuLtr) |
| Cloud Compute — Regular | 2 vCPU, 4 GB RAM, 80 GB SSD | $20/mo | Hourly, monthly cap | [Check the price](https://bit.ly/VuLtr) |
| High Frequency / High Performance | Faster NVMe-backed instances, higher clock speeds | Scales from the Regular entry points | Hourly, monthly cap | [Deploy this class](https://bit.ly/VuLtr) |
| Optimized Cloud Compute | CPU-, memory- and storage-optimized shapes | Scales from the Regular entry points | Hourly, monthly cap | [Compare shapes](https://bit.ly/VuLtr) |

Two practical notes on that table. The monthly number is a cap, not a commitment — an instance that runs ten hours bills for ten hours. And the smallest tier at roughly $2.50 a month is genuinely enough for a static site, a small API or a VPN endpoint; you do not need to spend more to get a working server.

GPU pricing is separate and metered per GPU-hour:

| GPU | Listed starting rate | ≈ hours covered by $300* |
| --- | --- | --- |
| NVIDIA A100 PCIe | $1.290/GPU-hr | ~232 |
| NVIDIA L40S | $1.712/GPU-hr | ~175 |
| AMD Instinct MI325X | $1.850/GPU-hr | ~162 |
| AMD Instinct MI355X | $1.990/GPU-hr | ~151 |
| NVIDIA HGX H100 | $2.300/GPU-hr | ~130 |

\*Only if your GPU instance type counts as an eligible "select product" for promotional credit. Confirm that before you budget around it.

Vultr also takes reservations for NVIDIA HGX B200 systems and clusters of AMD Instinct MI300X, MI325X and MI355X hardware, and it has deployed Nvidia GB300 NVL72 racks for larger AI workloads. Those are quoted rather than listed at a flat hourly rate, so treat the table above as the on-demand entry point.

## 50% off: the real math, and the two-invoice ceiling

The 50% promotion has a different flow. You create an account, pick a credit amount (**$10, $25, $50 or $100**), add a payment method, pay, and deploy. The discount then appears on your first two invoices — 50% off each one.

Vultr's own example: a $10 monthly invoice gets $5 deducted from the amount due. So if you run a $10/month server, the promotion saves you **$10 in total**, ever.

The limit is built into the terms. It expires after your first two invoices, and invoices are generated on the **first of each month**, not 60 days after signup. Sign up on the 28th and your first discounted invoice covers roughly three days of usage, which makes the promotion nearly worthless unless you scale up immediately. Sign up on the 2nd and you get close to two full months of discount.

The ceiling is what matters for comparison. Halving two invoices saves 50% of whatever those two bills total. So:

- First two invoices total **$100** → you save $50. The $300 credit is six times better.
- First two invoices total **$400** → you save $200. The $300 credit still wins.
- First two invoices total **$600** → you save $300. It is a tie.
- First two invoices total **$1,000** → you save $500. The 50% promotion wins by $200.

**$600 across two months is the crossover point.** Below it, take the credit code. Above it, take the 50% promotion. 👉 [Start the 50% off flow here](https://vultr.com/50off?ref=9738262-9J)

## Which deal fits your situation

**A week of testing, a demo, or a one-off migration.** Take FLY300VULTR. You are not paying anything for the credit, and $300 covers a lot of small instances: at $5/month for a 1 GB server, that is 60 instance-months of usage if this product type qualifies for credit. You will almost certainly never exhaust it.

**A production workload you plan to keep.** Run the crossover math first. If your first two months will bill under $600, the credit code is the better deal and simpler to use. If you are moving a real application with several instances and steady traffic, two months at 50% off usually beats a flat $300.

**You were going to fund the account anyway.** VULTRMATCH is the cleanest option: deposit $100, get $100 of bonus credit, and the $100 you put in is still yours. The $100 bonus is smaller than the $300 code, so this only wins if you value keeping your own balance intact and dislike the "select products" ambiguity that comes with promotional credit.

**GPU experiments.** Do the arithmetic before choosing. $300 buys roughly 151 hours on a single MI355X at the listed $1.99 per GPU-hour, which is six days of continuous runtime. The 50% promotion instead scales with your actual bill, so a heavy GPU week pushes you past the $600 crossover quickly. Either way, confirm GPU instances are eligible for whichever credit you pick, since promotional credit is restricted to select products.

## Where people get tripped up

- **Duplicate accounts are disqualified.** Vultr states plainly that duplicate accounts are not eligible for promotions. If you have ever had an account, none of these offers apply to you.
- **The codes do not stack.** Each one carries the line "cannot be combined with any other offers." The 50% page says nothing about stacking either, so plan your budget around using exactly one.
- **Promotional credit is not cash.** It applies to select products only and does not convert to a balance you can withdraw or apply anywhere.
- **The 50% promotion requires an upfront credit purchase.** You pay for $10 to $100 of account credit before the discount applies. The credit codes do not ask for a deposit.
- **No expiry date is published.** The coupon page lists no end date, and the 50% page says only "available for a limited time." If a code is what you want, use it while it is on the page.
- **Hourly billing means small mistakes stay small.** An instance left running over a weekend costs cents at the entry tier, not a surprise invoice.

## Is Vultr going to be around next year?

That is the fair question when a $300 credit comes from a company you have not used before. Vultr closed a growth financing round reported in November 2026 at a **$3.5 billion valuation**, led by LuminArx Capital Management and AMD Ventures, with Goldman Sachs as financial advisor; the Wall Street Journal put the round at **$333 million**. The stated use of funds is more GPUs and broader cloud capacity.

The hardware commitments are concrete. HPE announced a **$1.2 billion order** from Vultr in September 2026 for AMD Helios AI Rack systems — HPE's first order for that platform — with each rack carrying 72 AMD Instinct MI455X GPUs connected over UALink over Ethernet. Vultr has offered AMD Instinct MI300X since September 2024, was among the first clouds to deploy MI325X and MI355X, runs Nvidia H100 and GH200, chose HPE-built Nvidia GB300 NVL72 racks in June 2026, and committed over $1 billion to a 24,000-GPU MI355X cluster in Springfield, Ohio. It operates **32 data center regions across six continents** and was founded in 2014.

None of that guarantees anything, but it rules out the "guy with a reseller account" scenario. AMD is both an investor and a supplier, which is the strongest signal in the pile that the GPU roadmap has backing behind it.

## FAQ

**Where do I enter a Vultr promo code?**
The coupon page presents each offer as a "Use Code" for new sign-ups, so it is applied when you open the account. The 50% promotion works differently: you create the account, choose a credit amount, add a payment method, and pay; the discount then shows on your invoices.

**Do I have to make a deposit to get the $300?**
The coupon page does not ask for one. The 50% promotion does — you buy $10 to $100 of account credit as part of the flow.

**Can I use the 50% promotion and a credit code together?**
The credit codes explicitly cannot be combined with any other offer, and the 50% page does not say it stacks. Assume one or the other.

**How long does the 50% discount last?**
Two invoices. Invoices are generated on the first of each month, and the promotion expires after the second one.

**What happens when the credit runs out?**
Your account reverts to normal billing at the listed rates. There is no separate renewal price for promotional credit, so budget from the hourly rates above.

**Can I open a second account to use a code twice?**
No. Duplicate accounts are not eligible for promotions.

## Before you sign up

Pick by spend, not by the size of the headline number:

- **Under $600 across two months** → FLY300VULTR, the $300 credit.
- **Over $600 across two months** → the 50% off promotion, which scales with your bill.
- **Funding the account with $100 regardless** → VULTRMATCH, and keep your deposit.

Two things to confirm first: that you have never held a Vultr account, and that the instance type you plan to run counts as an eligible product for promotional credit. If both check out, 👉 [open the account and apply the $300 code](https://bit.ly/VuLtr) — or pick the 50% route if your first two invoices will clear $600.
