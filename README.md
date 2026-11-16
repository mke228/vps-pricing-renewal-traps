# Buy VPS Linux: What $6.49–$13.99 a Month Actually Buys, Why Renewal Prices Jump 1.8–2.2×, and Which Plan Fits a Blog, Docker Stack or VPN

A 4 GB Linux VPS currently lists at €8.30/mo at one host, $8.79/mo on a 24-month prepay at another, and $13.99/mo month-to-month at a third. The 2 GB tier sells for $7.99/mo, and one provider knocks the first month down to $1. The advertised number is where the comparison starts. What decides your bill over two years is the renewal rate behind it, how traffic is metered, and two or three limits that only appear in the FAQ.

Every price below comes from the providers' own plan pages. Where a page is old or silent on something, I say so rather than filling the gap.

> **Short version:** 1–2 GB of RAM covers a blog, a WireGuard tunnel or a chat bot. 4 GB runs a small Docker stack (Nextcloud, n8n, a reverse proxy and its database). Go to 8 GB and above once the box also serves production traffic. If you'd rather test two sizes before committing to one, Vultr's coupons page currently lists $300 in credit for new accounts, code FLY300VULTR, restricted to select products and not combinable with other offers: 👉 [claim the $300 credit and check which instance families it covers](https://bit.ly/VuLtr).

## The $300 credit, line by line

The credit is a promotional balance sitting next to your own funds, not a discount applied to a plan. Vultr's coupon page currently lists four new-customer offers:

| Code | What you get | Eligibility | Terms that matter |
| --- | --- | --- | --- |
| FLY300VULTR | $300 free credit | New customers only | Select products only, cannot be combined with other offers |
| 250VULTRFLY | $250 free credit | New customers only | Same restrictions |
| FLYTWOHUNDRED | $200 free credit | New customers only | Same restrictions |
| VULTRMATCH | Dollar-for-dollar match on your first deposit, up to $100 | Anyone new to Vultr | Expires 12 months after issue, applied 50/50, duplicate accounts excluded |

Two details change how you should use this. Codes can't be stacked, so you pick one and lose the others. And the match offer is applied on a 50/50 basis: on a $10 accrued balance, $5 comes out of the promotional credit and $5 out of your own money. To consume the full $100 match you have to push $100 of your own through the account as well, which makes it a rebate on spending rather than a free trial.

The free-credit codes are listed as applying to select products only. Vultr sells compute across several families (Cloud Compute, Optimized Cloud Compute, GPU and bare metal) with per-family pricing chosen at deploy time, so the honest move is to check the qualifying list before you launch anything expensive, then confirm the price on the deploy screen. 👉 [Open an account and apply one code before your first deploy](https://bit.ly/VuLtr).

## What the same money buys elsewhere right now

Prices in euros and dollars are not converted here. Compare inside one currency, and read the last column before the first.

| Plan | vCPU · RAM | Disk | Advertised price | Renewal / next term |
| --- | --- | --- | --- | --- |
| Hostinger KVM 1 | 1 · 4 GB | 50 GB NVMe | $6.49/mo, 24-month prepay ($155.76 today) | $11.99/mo for the next 24 months |
| Hostinger KVM 2 | 2 · 8 GB | 100 GB NVMe | $8.79/mo, 24-month prepay ($210.96) | $14.99/mo |
| Hostinger KVM 4 | 4 · 16 GB | 200 GB NVMe | $12.99/mo, 24-month prepay ($311.76) | $28.99/mo |
| Hostinger KVM 8 | 8 · 32 GB | 400 GB NVMe | $25.99/mo, 24-month prepay ($623.76) | $49.99/mo |
| Contabo CLOUD VPS 4 | 4 · 8 GB | 100 GB SSD | €4.40/mo for the first 24 months (list €5.50) | Not published |
| Contabo CLOUD VPS 6 | 6 · 12 GB | 200 GB SSD / 100 GB NVMe | €6.00/mo for the first 24 months (list €7.50) | Not published |
| Contabo CLOUD VPS 8 | 8 · 24 GB | 300 GB SSD / 150 GB NVMe | €11.20/mo for the first 24 months (list €14.00) | Not published |
| Contabo CLOUD VPS 12 | 12 · 48 GB | 400 GB SSD / 200 GB NVMe | €20.00/mo for the first 24 months (list €25.00) | Not published |
| Infrawire VPS Entry | not listed · 4 GB | NVMe | €8.30/mo, monthly billing | Same rate, no contract |
| Infrawire VPS Bronze | 4 · 8 GB | NVMe | €14.55/mo | Same rate, no contract |
| Infrawire VPS Silver | not listed · 16 GB | NVMe | €27.60/mo | Same rate, no contract |
| Infrawire VPS Gold | not listed · 24 GB | NVMe | €41.48/mo | Same rate, no contract |
| Infrawire VPS Platinum | not listed · 32 GB | NVMe | €52.20/mo | Same rate, no contract |
| buyvps S-2 | 1 · 2 GB | 30 GB NVMe RAID10 | $7.99/mo, first month $1 | $7.19/mo on annual billing |
| buyvps S-4 | 2 · 4 GB | 60 GB NVMe RAID10 | $13.99/mo, first month $1 | $12.59/mo on annual |
| buyvps S-8 | 3 · 8 GB | 120 GB NVMe RAID10 | $24.99/mo, first month $1 | $22.49/mo on annual |
| buyvps D-4 (dedicated CPU) | 1 · 4 GB | 45 GB NVMe RAID10 | $37.00/mo | $31.45/mo on annual |

Infrawire publishes RAM per plan but not vCPU and disk for every tier; the Bronze order summary shows 4 vCPU and 8 GB. Two plans at $8 don't buy the same machine: Infrawire's €8.30 entry gives 4 GB of RAM, Hostinger's $6.49 entry gives 4 GB plus a fixed traffic allowance, and buyvps's $7.99 gives half the RAM but unlimited traffic on NVMe RAID10.

## The renewal price is the real price

Hostinger is the one provider in this group publishing both numbers, which makes the arithmetic possible. KVM 1 goes from $6.49 to $11.99/mo, a 1.85× jump. KVM 4 goes from $12.99 to $28.99, which is 2.23×. On a 24-month cycle you pay $155.76 today and $287.76 for the term after, so four years on the smallest plan costs about $443 rather than the $156 the headline suggests. On KVM 4 the same four years come to roughly $1,007.

Contabo uses a different convention: €4.40, €6.00, €11.20 and €20.00 are all labelled "for the first 24 months" against crossed-out list prices of €5.50, €7.50, €14.00 and €25.00. The page doesn't state what happens after month 24. Don't extrapolate a renewal figure from the discount; budget from the crossed-out list price, which is the only upper bound the page gives you.

Infrawire and buyvps bill monthly at the listed rate with no long commitment, so the number you see is the number you keep paying. For a first VPS that lasts longer than a year, a €14.55 monthly plan can end up cheaper than a $6.49 plan that renews at $11.99, and you keep the option to leave.

## Three ways to say "unmetered traffic"

The same vCPU count can hide a fourfold difference in network capability, and this is where cheap plan lists get vague.

Contabo keeps traffic unlimited but raises the port speed with the tier: 200 Mbit/s on CLOUD VPS 4, 300 Mbit/s on VPS 6, 600 Mbit/s on VPS 8, 800 Mbit/s on VPS 12. Hostinger meters transfer instead: 4 TB, 8 TB, 16 TB and 32 TB per month on a 1 Gbps port. Infrawire advertises up to 10 Gbps with unmetered traffic across all five plans. buyvps lists unlimited traffic on every standard and dedicated plan.

What that means in practice: a nightly backup or a media-heavy site cares about port speed, while an API or bot cares about the transfer cap, and both care about what an overage costs. Hostinger's allowance is generous enough that a small site will never touch it. A 200 Mbit/s port is fine for a blog and painful for pushing container images or serving video.

## Limits that live in the FAQ

buyvps restricts outbound mail by default. Sending requires emailing support with your use case and getting the block lifted, which is a five-minute annoyance if you know about it and a lost afternoon if you don't. Reverse DNS is settable from the panel. The provider also gives every VPS its own kernel, so you can load modules and recompile without touching a neighbour.

Atlantic.Net charges separately for the pieces people assume are included: cPanel licensing from $23/mo and extra IPv4 addresses at $3.65/mo ($0.005431/hr). That page is dated 28 March 2023, so treat its plan prices as stale and the structure as the useful part. Any "$8 all-in" expectation deserves the same scrutiny everywhere.

Hostinger advertises "cancel anytime" next to its 24-month prepay without stating a refund for unused months. Assume prepaid money is committed money until a provider says otherwise in writing. Infrawire is explicit in the other direction: 7-day money-back guarantee on the first payment only.

## Match the plan to the job

- **Blog, static site, WireGuard, Telegram bot:** 1–2 GB is plenty. buyvps S-2 at $7.99/mo or Infrawire Entry at €8.30/mo for 4 GB if you want headroom for a database later.
- **A handful of containers (Nextcloud, n8n, reverse proxy, Postgres):** 4–8 GB. Contabo CLOUD VPS 4 gives 8 GB for €4.40 during the first 24 months, Hostinger KVM 2 gives 8 GB for $8.79 on prepay, Infrawire Bronze gives 4 vCPU and 8 GB for €14.55 monthly.
- **Production web app plus database plus a worker:** 8 GB and up, and look at dedicated CPU once response times start to matter. buyvps prices that jump openly: $24.99/mo for 3 shared vCPU and 8 GB against $69.00/mo for 4 dedicated vCPU and 8 GB. Shared cores handle bursty web traffic fine; a build server or a game server does not.
- **k3s or a small cluster:** the requirement is an independent kernel and an API you can drive from Terraform or Ansible. buyvps states both, and publishes 122,959 4K random read IOPS and 87,730 4K random write IOPS on a dedicated-CPU instance with NVMe RAID10 in Amsterdam, median of five fio runs. Those numbers matter more than core count if you're running etcd.

## Questions that come up before the first order

**Can I install my own ISO?** On buyvps, yes: upload a 64-bit ISO in the panel, attach it as a virtual CD-ROM, boot from it. Prebuilt images cover Ubuntu 22.04, 24.04 and 26.04 LTS, Debian 11 through 13, AlmaLinux 8 to 10, Rocky, CentOS Stream, Oracle Linux, Fedora 43 and 44, and openSUSE. Ask any other host directly; not all allow it.

**Will Docker and Kubernetes run?** Yes on any KVM plan with root access. k3s on shared vCPU is fine for a lab. For anything carrying traffic, dedicated CPU or a larger shared plan.

**I broke SSH with a firewall rule.** Infrawire offers a browser console from the client area that works when SSH doesn't; buyvps offers rescue mode for filesystem checks and root password recovery, plus reinstall in roughly 30 seconds to a minute. Check that a console exists before you buy, because a locked-out VPS with no console means a support ticket and a wait.

**What happens if I want out?** Infrawire refunds the first payment within 7 days. Contabo requires no notice on prepaid contracts and four weeks on post-paid ones. Hostinger's page doesn't describe refunds for the prepaid term.

## Before you pay

Three things decide whether a cheap Linux VPS stays cheap: the renewal price and its term, whether outbound mail is open if you plan to send any, and whether snapshots or backups are included or billed monthly on top. Get those three answers in writing, then pick the smallest plan that fits the job and let the credit or the monthly billing absorb your mistakes.

If you want to compare instance sizes on the same account rather than guessing, the $300 credit does that job: 👉 [start on Vultr with a new-customer credit code](https://bit.ly/VuLtr), confirm which products the credit covers, and size the box from real usage instead of a spec sheet.
