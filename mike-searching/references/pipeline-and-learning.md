# Pipeline, records, and learning

Use this reference when the user asks to save, update, prioritize, forecast, review, or learn from partnership activity. The schema is reusable; do not place real customer records in this skill package.

## 1. Object model

- `Account` = company, media outlet, creator business, store, facility, or organization.
- `Contact` = person connected to the Account.
- `Opportunity` = a specific test, content collaboration, sponsorship, pilot, resale, distribution, or purchase path.
- `Interaction` = an email, message, call, meeting, reply, redirect, proposal, or other dated touch.
- `Outcome` = publish, pilot result, order, repeat order, rejection, failure, or other measurable result.

Keep Account, Contact, and Opportunity separate. One account may have several contacts and opportunities. Never overwrite a confirmed fact with a guess.

## 2. Pipeline

Use the narrowest accurate stage:

`发现 → 初筛 → 已研究 → 准备开发 → 已联系 → 已回复 → 已确认需求 → 会议 → Pilot → 商务谈判 → 合同 → 首单 → 交付 → 测试 → 复购 → 长期客户 / 暂停 / 拒绝`

For creator/media work, use the same backbone and record the relevant equivalent: test proposal, content planning, test, publish, attribution, and repeat collaboration.

Move a record only when evidence supports the move. A reply is not automatically a qualified opportunity; a meeting is not automatically a pilot; a pilot is not automatically a first order.

Use this minimum mapping for common replies:

- `NO_REPLY` → `已联系` (keep the last outreach date and next follow-up date).
- `INTERESTED` or a factual information request → `已回复`; move to `已确认需求` only after the recipient confirms a real problem, use case, timing, market, quantity, or procurement process.
- `PRICING_REQUEST` → `已回复`; it becomes `商务谈判` only after scope and commercial variables are confirmed and a real buying path exists.
- `SAMPLE/PILOT` → `Pilot` only after fit, timing, conditions, deliverables, rights, support, and value exchange are accepted.
- `REJECTED` or `DO_NOT_CONTACT` → `拒绝`.

Never promote an opportunity solely because a recipient asked for a catalog, replied quickly, attended a meeting, or has a large audience.

## 3. Minimum record fields

Use generic fields and placeholders in reusable examples:

### Account

`account_id`, `name`, `archetype`, `country/market`, `website`, `source_urls`, `customer/audience type`, `product/category fit`, `evidence status`, `owner`, `notes`

### Contact

`contact_id`, `account_id`, `role`, `working language`, `contact route`, `role evidence`, `last verified date`, `consent/do-not-contact status`

Do not put personal phone numbers, private emails, addresses, or message contents in a public skill package.

### Opportunity

`opportunity_id`, `account_id`, `contact_id`, `type`, `value track`, `stage`, `problem/use case`, `harvest or procurement timing`, `deliverables`, `content rights`, `commercial terms`, `cash/contribution EV`, `strategic/authority upside`, `forecast with confidence`, `decision`, `next action`, `review date`, `failure reason`

### Interaction

`date`, `channel`, `direction`, `summary`, `evidence/status`, `recipient state`, `forecast change`, `commitment`, `next action`, `owner`, `due date`

Record summaries and decision-relevant facts, not unnecessary private conversation detail.

## 4. Follow-up queue

Every active opportunity needs:

- one owner;
- one next action;
- one due/review date;
- one reason the action is useful now;
- one stop or park condition.

Prioritize by expected attributable value, urgency/time window, probability of the next stage, effort, and opportunity cost. Do not prioritize only by age, reply speed, follower count, or prestige.

## 5. Forecast and decision log

For each material decision record:

`date`, `evidence snapshot with source URLs/dates`, `score`, `probabilities with evidence and confidence`, `cash/contribution EV`, `strategic/authority upside`, `decision`, `authorized terms`, `unknowns`, `override`, `owner`, and `review trigger`.

When new evidence arrives, show what changed: stage, probability, EV, risk, or decision. Preserve the prior forecast so prediction error can be measured.

For commercial conditions, use this source priority: latest explicit user authorization → latest formal quote/contract → current official commercial source. Historical snapshots are not current authorization. If a current price, freight, tax, MOQ, payment, warranty, delivery, territory, or exclusivity term is not confirmed, leave it `UNKNOWN` and pause the decision.

## 6. Outcome and failure taxonomy

Measure downstream outcomes, not just activity:

- attributable revenue and contribution profit;
- qualified opportunity and first order;
- repeat order, LTV, and channel expansion;
- published evidence, backlink/SEO value, authority, and usable customer insight;
- cost, time, machine utilization, freight, support, and opportunity cost.

Record a failure reason when known, for example:

`poor fit`, `no purchase intent`, `wrong contact`, `timing`, `price/terms`, `capacity`, `fulfillment`, `support burden`, `content mismatch`, `unreliable execution`, `legal/market constraint`, or `insufficient evidence`.

## 7. Learning loop

Use:

`Execution → Record → Outcome → Prediction Error → Hypothesis → Experiment → Rule Update → New Version`

Compare predicted and actual reply, meaningful conversation, pilot, publish, first-order, sales, and repeat rates. A higher reply rate is not a success if Revenue, Creator ROI, Qualified Opportunity, or Contribution Margin falls.

Update the system only when the pattern is supported by multiple observations or a deliberate experiment. Keep a hypothesis separate from a confirmed rule.

## 8. Cross-learning

Share only generalized, de-identified lessons:

- creator objections can improve B2B messaging;
- B2B objections can suggest creator education topics;
- commercial grower feedback can improve product positioning;
- retailer questions can improve creator resources;
- creator conversion can inform channel strategy;
- B2B orders can change creator resource allocation.

Never move a person's name, private message, address, or confidential terms into the generalized rule.
