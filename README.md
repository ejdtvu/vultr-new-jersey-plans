# Vultr New Jersey: Which Plans You Can Actually Deploy, What They Cost With Backups and DDoS, and Who Should Skip It

Vultr has a New Jersey region, and it sits inside the provider's New York Metro footprint, which makes it the location to pick for visitors in NYC, northern New Jersey and the wider East Coast. Cloud Compute there starts at **$5/mo** for 1 vCPU, 1 GB RAM, 25 GB SSD and 1 TB of transfer, and there is a **$2.50/mo** IPv6-only instance that Vultr only sells in a couple of US locations, so New Jersey availability needs checking before you build around it. What follows is the full plan list for the region, the add-on fees that decide your real monthly bill, the point where New Jersey bare metal runs out of headroom, and the cases where a different provider is the better call.

One caveat that applies to every number below: the prices come from a third-party price tracker (WebHostingBreak, page dated 17 September 2026), not from Vultr's own pricing page, and they were not cross-checked against it. Treat them as accurate-enough for planning and confirm at checkout.

## The short answer for most readers

> Cloud Compute Regular 1 vCPU / 1 GB at **$5/mo** covers a small site, an API, a Discord bot, a staging box or a monitoring node. If the box will hold a database or serve production traffic, go to the **$24/mo** tier instead: High Frequency 2 vCPU / 4 GB with 128 GB NVMe, or High Performance AMD 2 vCPU / 4 GB with 100 GB NVMe. Same price, newer CPUs, far more fast disk than the $20 Regular plan.

👉 [See the current New Jersey plan list and prices](https://bit.ly/VuLtr)

## All 17 plans listed for New Jersey (and the four that are not)

Five columns, one caveat: not every plan is sold in every region. The four bare metal rows marked Chicago were not available in New Jersey on the page these figures came from.

| Plan | vCPU / RAM / Storage | Price (USD/mo) | Location | Order |
| --- | --- | --- | --- | --- |
| Cloud Compute Regular 1 vCPU / 0.5 GB (IPv6 only) | 1 / 0.5 GB / 10 GB SSD | $2.50 | New Jersey | [Order](https://bit.ly/VuLtr) |
| Cloud Compute Regular 1 vCPU / 1 GB (most popular) | 1 / 1 GB / 25 GB SSD | $5 | New Jersey | [Order](https://bit.ly/VuLtr) |
| High Frequency 1 vCPU / 1 GB (Intel, NVMe) | 1 / 1 GB / 32 GB NVMe | $6 | New Jersey | [Order](https://bit.ly/VuLtr) |
| High Performance AMD 1 vCPU / 1 GB (EPYC, NVMe) | 1 / 1 GB / 25 GB NVMe | $6 | New Jersey | [Order](https://bit.ly/VuLtr) |
| Cloud Compute Regular 1 vCPU / 2 GB | 1 / 2 GB / 55 GB SSD | $10 | New Jersey | [Order](https://bit.ly/VuLtr) |
| Cloud Compute Regular 2 vCPU / 2 GB | 2 / 2 GB / 65 GB SSD | $15 | New Jersey | [Order](https://bit.ly/VuLtr) |
| Cloud Compute Regular 1 vCPU / 1 GB + DDoS Protection (10 Gbps) | 1 / 1 GB / 25 GB SSD | $15 | New Jersey | [Order](https://bit.ly/VuLtr) |
| Cloud Compute Regular 2 vCPU / 4 GB | 2 / 4 GB / 80 GB SSD | $20 | New Jersey | [Order](https://bit.ly/VuLtr) |
| High Frequency 2 vCPU / 4 GB (Intel, NVMe) | 2 / 4 GB / 128 GB NVMe | $24 | New Jersey | [Order](https://bit.ly/VuLtr) |
| High Performance AMD 2 vCPU / 4 GB (EPYC, NVMe) | 2 / 4 GB / 100 GB NVMe | $24 | New Jersey | [Order](https://bit.ly/VuLtr) |
| Cloud Compute Regular 4 vCPU / 8 GB | 4 / 8 GB / 160 GB SSD | $40 | New Jersey | [Order](https://bit.ly/VuLtr) |
| Bare Metal Intel Xeon E3-1270 | 4 cores / 32 GB / 480 GB SSD | $120 | New Jersey | [Order](https://bit.ly/VuLtr) |
| Bare Metal Intel Xeon E-2286G | 6 cores / 32 GB / 1920 GB SSD | $185 | New Jersey | [Order](https://bit.ly/VuLtr) |
| Bare Metal AMD EPYC 4245P (most popular) | 6 cores / 32 GB / 1920 GB NVMe | $295 | New Jersey | [Order](https://bit.ly/VuLtr) |
| Bare Metal AMD EPYC 4345P | 8 cores / 64 GB / 3890 GB NVMe | $365 | Chicago | [Order](https://bit.ly/VuLtr) |
| Bare Metal AMD EPYC 7443P | 24 cores / 256 GB / 960 GB SSD | $725 | Chicago | [Order](https://bit.ly/VuLtr) |
| Bare Metal AMD EPYC 9254 | 24 cores / 384 GB / 960 GB SSD | $825 | Chicago | [Order](https://bit.ly/VuLtr) |

Prices as listed by WebHostingBreak on 17 September 2026, USD per month, US New Jersey location unless marked. Every instance is billed hourly up to that monthly cap. Availability and price at the order page are what count.

## What "New Jersey" actually refers to at Vultr

Three different things get called New Jersey in Vultr coverage, and they matter for different reasons.

**The region.** New Jersey is a deployable availability zone inside the New York Metro area. That is the part that affects your latency to East Coast users, and it is the only part you can pick in the control panel.

**The office.** Vultr Holdings lists Matawan, New Jersey alongside West Palm Beach, Florida as its office locations, and the New Jersey address is the one most of its engineering hiring runs through: kernel and hypervisor development, network automation, cloud storage engineering, platform software, cloud security architecture, Linux systems administration. That tells you the New Jersey presence is not just a rack in a building; a chunk of the people who build the platform sit there.

**The facility.** A third-party data center directory lists a "Vultr Secaucus 47" facility in Secaucus, New Jersey, described as a 32 MW GPU cloud site built in 2022, Tier 4, 172,448 sq ft, PUE 1.51, air and rear-door cooling, 17% renewable energy, 38+ network carriers, 9+ fiber providers, an AWS cloud on-ramp, and certifications including FedRAMP, LEED and PCI-DSS. The same entry lists H100 and GH200 GPU infrastructure. None of that has been confirmed on Vultr's own pages, and other directory sites list further New Jersey facilities with specifications that contradict each other, including tier ratings that disagree within a single page. Use the Secaucus entry as a lead worth checking in the console, not as a published fact.

If you are ordering for a production cutover, check the status page the same day. Directory entries and maintenance notices age badly.

## The number that actually lands on your card

The sticker price is rarely the bill. Four add-ons change it, and all four are easy to forget until the first invoice.

- **Automatic backups:** +20% of the instance price.
- **Snapshots:** $0.05 per GB per month.
- **DDoS Protection:** +$10/mo per instance, for 10 Gbps of mitigation.
- **Bandwidth overage:** $0.01 per GB beyond the pooled quota.
- **Windows Server:** licensed at extra cost.

Two worked examples, using those published rates:

- The $5 Cloud Compute box with backups runs **$6/mo**. Add DDoS protection and it is **$16/mo**, more than triple the headline.
- The $20 2 vCPU / 4 GB box with backups runs **$24/mo**. Add DDoS and it is **$34/mo**. At that point you are within $10 of the $24 NVMe plan plus backups, which is a better machine.

There is no introductory discount and no renewal jump. What you see is what you keep paying. There is also no money-back guarantee and no free trial, so the way to test is hourly billing: destroy the instance and the meter stops. A two-day spike test on a $40 plan costs a few dollars.

Support runs 24/7 but through tickets only. No live chat, no phone line, and a large documentation library standing in for a human. The 100% uptime SLA is settled in service credits, not cash, which is compensation terms rather than a promise that nothing goes down.

👉 [Start with hourly billing and destroy the instance when the test is done](https://bit.ly/VuLtr)

## Which plan fits which job

**A small site, a bot, an internal tool, a dev box.** Regular Performance at $5 or $10. It runs previous-generation Intel CPUs on standard SSD, which is fine for anything that is not disk-bound.

**Anything with a database, or production traffic.** Skip Regular and pay the extra $4. At $24 you get High Frequency 2 vCPU / 4 GB with **128 GB NVMe**, or High Performance AMD with **100 GB NVMe** on EPYC. The $20 Regular equivalent gives you 80 GB of standard SSD for only $4 less. On disk throughput alone the NVMe plans are the better buy.

**IPv6-only experiments.** The $2.50 plan is 0.5 GB RAM and 10 GB SSD, no IPv4. Any project that needs an IPv4 address cannot use it, and it is only deployable in a couple of US locations, so check New Jersey availability before planning around it.

**Dedicated vCPUs for CPU-bound work.** Optimized Cloud Compute exists for this. No pricing for it in the data behind this article, so confirm in the console.

**GPU work.** The Secaucus directory entry lists H100 and GH200, and Vultr sells cloud GPUs as a product line. No verified GPU model list or hourly rate was available for this article, so check the console for current GPU shapes and pricing before you budget.

**Big single-tenant boxes.** New Jersey tops out at the $295 AMD EPYC 4245P with 6 cores, 32 GB RAM and 1920 GB NVMe. The 64 GB, 256 GB and 384 GB EPYC machines in the list are Chicago. If you need 64 GB or more of RAM on bare metal and you need it in New Jersey, this table does not give it to you, and that is a real constraint for memory-hungry databases.

👉 [Compare the High Frequency and High Performance plans side by side](https://bit.ly/VuLtr)

## Who should not buy this

Vultr is self-managed. There is no cPanel bundle, no managed WordPress, no shared hosting, and nobody will log in and fix your stack. If you want a host that installs WordPress and answers the phone, this is the wrong product and you will spend more time than money.

It is also the wrong choice if you need a refund window to feel safe, if bank transfer is your only payment method (cards, PayPal and crypto are accepted, transfer is not), or if Windows Server licensing bundled into the price is a requirement.

## FAQ

**Which region is New Jersey in?**
New York Metro. Pick it for East Coast US users, and expect it to be the sensible default over Chicago for anything serving NYC.

**Can I run the $2.50 plan in New Jersey?**
It is IPv6-only with 0.5 GB RAM and 10 GB SSD, and Vultr only sells it in a couple of US locations. Confirm the region at the order page; if your project needs IPv4, it is unusable regardless.

**Will the price go up after the first term?**
No introductory pricing means no renewal shock. The listed price is the ongoing price. Add-ons still apply on top.

**Can I get a refund if I do not like it?**
There is no money-back guarantee on record. Hourly billing is the substitute: destroy the instance, charges stop.

**What payment methods work?**
Visa and Mastercard, PayPal, and cryptocurrency. Accounts are prepaid or charged to a card.

## The decision, in one pass

Only need a small Linux box on the East Coast, with a real IPv4 address and no drama: the **$5 Cloud Compute Regular 1 vCPU / 1 GB**.

Running a database, a container host or anything where disk speed shows up in response times: the **$24 High Frequency 2 vCPU / 4 GB** with 128 GB NVMe, or the High Performance AMD equivalent if you prefer EPYC.

Need a single-tenant machine in New Jersey: the **$120 Xeon E3-1270** is the entry point, and **$295** is the ceiling before you have to move regions.

Before you order, two checks: confirm the plan you want is actually sold in the New Jersey region, because not every plan is available in every location, and confirm whether you need IPv4, because the cheapest tier does not include it.

👉 [Check New Jersey availability and current pricing before you deploy](https://bit.ly/VuLtr)
