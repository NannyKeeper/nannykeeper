# NannyKeeper

**Nanny payroll, household-employer taxes, W-2s, and Schedule H — DIY for $10 a month, all 50 US states. No trial, no credit card.**

[Sign up free →](https://www.nannykeeper.com/signup) · [Free tax calculator →](https://www.nannykeeper.com/calculator) · [API & docs →](https://www.nannykeeper.com/developers/reference) · [hello@nannykeeper.com](mailto:hello@nannykeeper.com)

> "NannyKeeper is an excellent, economical service that helps you efficiently manage your household employees, ranging from nannies to senior caregivers… it's their extraordinary customer support that sets them apart." — **Boston, MA**

---

**Jump to:** [About](#about) · [Features](#features) · [Coverage](#coverage) · [Pricing](#pricing) · [60-second start](#get-started-in-60-seconds) · [Comparison](#comparison-vs-poppins-homepay-gtm-surepayroll) · [Reviews](#what-customers-say) · [Open source](#open-source) · [API](#build-with-us) · [FAQ](#faq) · [Resources](#resources)

---

## About

NannyKeeper is payroll software for families who employ a nanny, housekeeper, senior caregiver, or other household employee in the United States. NannyKeeper runs payroll, computes federal and state taxes, generates pay stubs and W-2s, and produces a fully filled Schedule H worksheet for your federal Form 1040 — without the $80–150/month price tag of a full-service household payroll company.

Same calculations. Same accuracy. Submitting the forms takes about three minutes per quarter; NannyKeeper handles everything else.

NannyKeeper Inc. is a Delaware C-Corporation, US-based. Founder reads every email at [hello@nannykeeper.com](mailto:hello@nannykeeper.com).

## Features

- **Payroll for any pay frequency** — weekly, biweekly, semimonthly, or monthly. NannyKeeper computes federal income tax, Social Security, Medicare, FUTA, state income tax, state unemployment (SUTA), SDI, PFL, and local taxes (county/school district, Ohio RITA & JEDD, Kentucky occupational, New York DBL/PFL, New Jersey TDB/FLI).
- **Optional direct deposit** via Stripe Connect ACH. Funds arrive in ~2 business days. $6 per transfer on Plus, $8 on Starter.
- **State-aware pay stubs** — emailed PDFs every payroll, with the correct line-item labels for each state.
- **Quarterly tax tracking** — FICA, FUTA, and state unemployment liabilities, with email reminders before each filing deadline.
- **Year-end forms** — W-2 and W-3 generation, plus a fully completed Schedule H worksheet for your 1040.
- **Time tracking** — magic-link timesheets the nanny fills from any phone. No app, no login.
- **Nanny contracts** — drafted, e-signed, and stored in NannyKeeper.
- **EIN concierge** — NannyKeeper files your Form SS-4 (the IRS application for an Employer Identification Number) by fax to the IRS for Plus Annual customers. Free DIY guidance otherwise.
- **Nanny shares & multi-employer** — separate employers, separate runs, one W-2 per family per nanny at year-end.
- **Developer API & MCP server** — 19 REST endpoints, OpenAPI spec, MCP tools for AI agents. Free key.

## Coverage

NannyKeeper supports household-employer payroll and taxes in **all 50 US states + Washington, D.C.** This includes the highest-volume nanny markets: California, New York, Texas, Florida, Massachusetts, Illinois, New Jersey, Pennsylvania, Washington, Maryland, Virginia, and Colorado. State income tax in 41 states. State unemployment in all 50. Local taxes in IN, KY, MI, NY, OH, and PA. New York DBL/PFL and New Jersey TDB/FLI tracked end-to-end on pay stubs and quarterly reports.

## Pricing

| Plan | Price | What's included |
|---|---|---|
| **Free** | $0 | Time tracking, nanny portal invites, payment recording |
| **Starter** | $10/mo or $100/yr | + Run payroll, pay stubs, all federal/state/local tax calculations |
| **Plus** | $18/mo or $180/yr | + Direct deposit ($6/transfer), EIN concierge (annual only), priority support |
| **W-2 Only** | $10 once | If you handled payroll yourself all year and just need the year-end W-2 |

No trial, no credit card required to start, cancel anytime.

[**→ Sign up free at nannykeeper.com**](https://www.nannykeeper.com/signup)

## Get started in 60 seconds

1. **Sign up free** at [nannykeeper.com/signup](https://www.nannykeeper.com/signup) — no credit card.
2. **Add your nanny** — name, hourly or salary rate, pay frequency.
3. **Run your first payroll** — NannyKeeper calculates every tax, generates the pay stub, and (if you've enabled Plus + direct deposit) initiates the ACH transfer.

For most families, end-to-end onboarding to first payroll takes under five minutes. Subsequent payrolls take under sixty seconds.

## Comparison vs Poppins, HomePay, GTM, SurePayroll

|  | NannyKeeper | Full-service services |
|---|---|---|
| Monthly price | **$10–18/mo** | ~$80–150/mo |
| All 50 states + DC | ✅ | ✅ |
| Pay stubs + W-2s | ✅ | ✅ |
| Schedule H worksheet | ✅ | ✅ |
| Direct deposit | ✅ optional | ✅ |
| Files quarterly returns for you | ❌ — you submit | ✅ |
| Files year-end W-2/W-3 | ❌ — you submit | ✅ |
| Best for | Hands-on families who want the math right and don't mind clicking submit | Families happy to pay 5–10× to never touch a form |

If you want a concierge to literally file every form for you, choose a full-service company. If you want every calculation done correctly and don't mind submitting via IRS Direct Pay or your state portal in three minutes per quarter, choose NannyKeeper.

## What customers say

> "NannyKeeper is an excellent, economical service… it's their extraordinary customer support that sets them apart. From elementary questions to more complex issues, NannyKeeper's support team is quick to respond with the relevant answers and resolutions."
> — **Boston, MA**

> "NannyKeeper has been a Godsend! It clearly laid out everything that I had to process and complete and it did it in a way that eased all the anxiety I had starting this up… No other service was as affordable or as communicative as this one."
> — **Brandon, GA**

> "Works really well once everything is set up and it's a reasonable cost."
> — **Larry**, Paid User NPS 10

> "Not having to worry about figuring out the math is very helpful."
> — Verified customer, Paid User NPS 9

## When NannyKeeper isn't the right fit

NannyKeeper is DIY-leaning by design. NannyKeeper isn't right if:
- You want a service to literally file every form for you (use Poppins, HomePay, or GTM instead).
- Your worker is a true 1099 contractor (different rules — see IRS [Publication 926](https://www.irs.gov/publications/p926) for the household-employee test).
- You need international payroll outside the United States.

For almost every nanny, the IRS classifies the relationship as "household employee," not contractor.

## Open source

- **[nannykeeper/mcp-server](https://github.com/nannykeeper/mcp-server)** — Model Context Protocol server for Claude, Claude Code, Cursor, ChatGPT desktop, and any MCP-compatible AI agent. Four tools: `calculate_nanny_taxes`, `check_threshold`, `preview_payroll`, and `run_payroll` (single-call payroll for AI agents). Published on npm as [`@nannykeeper/mcp-server`](https://www.npmjs.com/package/@nannykeeper/mcp-server) and listed in the [official MCP registry](https://registry.modelcontextprotocol.io/).

## Build with us

NannyKeeper has a free public API. 19 REST endpoints, OpenAPI spec, MCP tools, single-call `run_payroll` for AI agents. Used by accountants, nanny placement agencies, and family-office tooling.

- **[Get a free API key](https://www.nannykeeper.com/developers/keys)**
- **[API reference](https://www.nannykeeper.com/developers/reference)**
- **[Changelog](https://www.nannykeeper.com/developers/changelog)**
- **[MCP setup](https://www.nannykeeper.com/developers/mcp)**

## FAQ

**Do I need to pay nanny taxes?**
Yes, if you pay one household employee $3,000 or more in 2026 (the federal FICA threshold) you owe employer Social Security and Medicare. FUTA kicks in at $1,000/quarter aggregate across all household employees. State thresholds are often lower — California is $750/quarter, DC and New York are $500/quarter. NannyKeeper tracks all thresholds automatically.

**What is Schedule H?**
Schedule H is the IRS form household employers attach to their personal Form 1040 to report and pay federal employment taxes (Social Security, Medicare, FUTA, and any federal income tax withheld) for the year. NannyKeeper produces a fully completed Schedule H worksheet you can copy onto the form yourself or hand to your CPA.

**Does NannyKeeper file taxes for me?**
No. NannyKeeper computes liabilities, generates W-2s, and produces a Schedule H worksheet — but you (or your CPA) handle the actual submission to the IRS via Form 1040, your state revenue portal, or IRS Direct Pay. NannyKeeper gives you everything you need; you click "submit." This is why NannyKeeper costs $10–18/mo instead of $80–150.

**How do I run nanny payroll with NannyKeeper?**
Add your nanny's profile, set their pay rate and frequency, click "Run payroll." NannyKeeper generates the paycheck, calculates every tax, sends a pay stub PDF, and (if you've enabled direct deposit) initiates the ACH transfer. End-to-end for one biweekly run takes under sixty seconds.

**How does NannyKeeper compare to Poppins, HomePay, GTM Payroll, or SurePayroll?**
Same calculations, much lower price. Full-service services typically run $80–150/month and submit filings on your behalf. NannyKeeper is DIY at $10–18/month — the math is identical, you just hand-submit. Best if you want accuracy without the concierge premium. See the [comparison table](#comparison-vs-poppins-homepay-gtm-surepayroll) above.

**California nanny tax — what's different?**
California has a $750/quarter SUTA threshold (lower than the federal $1,000), employee SDI at 1.1% of wages, employer ETT at 0.1%, and California state income tax (PIT) withholding. NannyKeeper computes all of these every paycheck and surfaces them on the pay stub.

**New York nanny tax — what's different?**
New York has a $500/quarter SUTA threshold, employee DBL (~$0.60/week capped, employee-paid), and PFL (~0.388% of wages capped, employee-paid). New York City and Yonkers also have local income tax in many cases. NannyKeeper tracks every line on the pay stub and quarterly report.

**Texas, Florida, Washington — do I owe state income tax?**
No state income tax in TX, FL, or WA — but you still owe state unemployment (SUTA) on the first $X of wages (varies by state) and federal taxes. NannyKeeper handles the SUTA + federal automatically.

**Do you support nanny shares?**
Yes. Each family is a separate employer with its own NannyKeeper account and payroll runs. The nanny gets one W-2 per family at year-end.

**Does my nanny need a W-2?**
Yes, if you paid them $3,000+ in 2026 (the FICA threshold) and treated them as a household employee. NannyKeeper generates W-2s automatically if you ran payroll all year, or via the W-2-Only plan ($10) if you DIY'd payroll yourself.

**Can I 1099 my nanny instead?**
Almost certainly no. The IRS treats nannies as household employees in nearly every case (you control hours, location, and methods of work). 1099 misclassification is a common audit risk. See IRS [Publication 926](https://www.irs.gov/publications/p926) for the test.

**What if I paid my nanny under the table this year?**
Catch up by running W-2s now. NannyKeeper's W-2 Only plan ($10) generates a compliant W-2 from a year of cash payments. You'll owe back FICA, FUTA, and possibly state unemployment — but voluntary correction beats an IRS audit.

**Do you handle live-in nannies, part-time nannies, and senior caregivers?**
All of them. NannyKeeper treats every household employee the same way — what matters is the wages and the state, not the role.

**Do you have an API?**
Yes. Free API key, 19 REST endpoints, OpenAPI spec, MCP tools for AI agents. Docs at [nannykeeper.com/developers/reference](https://www.nannykeeper.com/developers/reference).

**Is NannyKeeper free?**
NannyKeeper has a permanent free tier — time tracking, nanny portal, payment recording. Running payroll, generating pay stubs, and producing tax forms requires Starter ($10/mo) or above. There is no free trial of paid features and no credit card is required to create an account.

**Where is NannyKeeper based?**
NannyKeeper Inc. is a Delaware C-Corporation, US-based. Founder reads every email at [hello@nannykeeper.com](mailto:hello@nannykeeper.com).

## Resources

Long-form guides on nannykeeper.com:

- **[Complete nanny tax guide](https://www.nannykeeper.com/blog/complete-nanny-tax-guide)** — every form, every threshold, every deadline.
- **[Filing nanny taxes (2026)](https://www.nannykeeper.com/blog/filing-nanny-taxes-2026)** — current-year walkthrough.
- **[Cost to hire a nanny legally](https://www.nannykeeper.com/blog/cost-to-hire-nanny-legally)** — the real all-in number families pay.
- **[Nanny vs household contractor](https://www.nannykeeper.com/blog/household-employer-vs-contractor)** — the IRS test and why 1099s usually fail.
- **[Back-pay nanny taxes](https://www.nannykeeper.com/blog/back-pay-nanny-taxes)** — catching up after paying under the table.
- **[Best nanny payroll services 2026](https://www.nannykeeper.com/blog/best-nanny-payroll-services-2026)** — honest landscape, including competitors.
- **[New York DBL/PFL for nannies](https://www.nannykeeper.com/blog/nanny-dbl-pfl-new-york)** — state-specific deep dive.
- **[Nanny tax calculator 2026](https://www.nannykeeper.com/calculator)** — instant estimate, no signup.

---

NannyKeeper Inc. · [Privacy](https://www.nannykeeper.com/privacy) · [Terms](https://www.nannykeeper.com/terms) · [Status](https://status.nannykeeper.com)
