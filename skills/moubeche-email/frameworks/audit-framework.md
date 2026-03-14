# Email Audit & Diagnosis Framework

## The Moubeche Diagnostic Rule [Moubeche principle]

| Symptom | Root Cause | Fix Domain |
|---------|-----------|------------|
| Open rate < 40% | Deliverability problem | Technical setup, domain reputation, warm-up |
| Open rate > 50% but reply rate < 3% | Copy problem | Subject line works, but body/CTA fails |
| Reply rate > 8% but no meetings | CTA problem | Ask is wrong, friction too high, or wrong audience |
| High unsubscribe (> 5%) | Targeting problem | Wrong audience or wrong message-market fit |
| Bounce rate > 5% | List quality problem | Email verification needed |
| Spam reports > 0.1% | Trust/frequency problem | Space touchpoints, improve relevance |

## Full Audit Checklist

### Layer 1: Technical Foundation
- [ ] SPF record configured correctly
- [ ] DKIM signing active
- [ ] DMARC policy set
- [ ] MX records valid
- [ ] Custom tracking domain (not shared ESP domain)
- [ ] Dedicated outreach domain (not main business domain)
- [ ] Email warm-up completed (3-5 weeks minimum)
- [ ] Sending volume: 40-100 emails/day per sender max
- [ ] Staggered sending (not bulk-blasted)
- [ ] No attachments (Google Drive links instead)
- [ ] Simple HTML signature (no complex layouts)
- [ ] Opt-out/unsubscribe mechanism present

### Layer 2: List Quality
- [ ] Email verification run (bounce rate < 2%)
- [ ] Contact data is recent (< 90 days old)
- [ ] Segments defined by pain point, not just demographics
- [ ] No purchased lists or scraped emails without verification
- [ ] Inactive contacts identified and separated

### Layer 3: Copy Quality
- [ ] Subject line: 1-8 words, casual tone, relevant
- [ ] Opening line: about the PROSPECT, not about you
- [ ] Body: 50-125 words (cold), 150-300 words (warm/nurture)
- [ ] Single clear CTA matched to trust level
- [ ] "You/your" count > "I/we/our" count
- [ ] No spam trigger words (FREE, GUARANTEED, ACT NOW, etc.)
- [ ] PAS or relevant framework applied
- [ ] Personalization beyond first name (context, pain, trigger)
- [ ] No multiple CTAs competing for attention

### Layer 4: Sequence Logic
- [ ] 4-9 follow-ups planned
- [ ] Each follow-up adds NEW value (no "just checking in")
- [ ] Timing: 2 days → 4 days → 4 days → 5+ days between steps
- [ ] Total sequence duration: 10-25 days
- [ ] Breakup email included as final step
- [ ] Follow-ups in same thread (no new subject line)
- [ ] Multichannel steps included (LinkedIn, phone)

### Layer 5: Strategy Alignment
- [ ] Audience awareness level identified
- [ ] Offer-to-audience match validated
- [ ] Email goal matches funnel stage (reply vs click vs purchase)
- [ ] Segmentation active (not one-size-fits-all)
- [ ] Metrics tracked: reply rate, booking rate, conversion rate
- [ ] A/B testing active on at least one variable
- [ ] Content/brand presence supports outbound (prospects can find you)

## Audit Output Format

When delivering an audit, structure it as:

```
## AUDIT VERDICT: [CRITICAL / NEEDS WORK / SOLID / STRONG]

### Score: X/10

### Top 3 Issues (ranked by revenue impact):
1. [Issue] — [Impact] — [Fix]
2. [Issue] — [Impact] — [Fix]
3. [Issue] — [Impact] — [Fix]

### Layer-by-Layer Analysis:
[Technical] — [Status] — [Details]
[List Quality] — [Status] — [Details]
[Copy] — [Status] — [Details]
[Sequence] — [Status] — [Details]
[Strategy] — [Status] — [Details]

### Priority Action Plan:
1. [Immediate fix — do today]
2. [This week]
3. [This month]

### Expected Impact:
[What these fixes should produce in metrics]
```

## Diagnostic Decision Tree

```
START: What's the problem?
│
├─ "Not enough opens"
│  └─ Check: deliverability setup → subject lines → sender reputation → list quality
│
├─ "Not enough replies"
│  └─ Check: copy quality → CTA strength → personalization depth → audience targeting
│
├─ "Replies but no meetings"
│  └─ Check: CTA clarity → follow-up process → offer-audience fit → sales handoff
│
├─ "Meetings but no deals"
│  └─ Check: qualification in emails → expectation setting → offer positioning
│
├─ "High unsubscribes"
│  └─ Check: frequency → relevance → targeting → value delivery
│
├─ "Going to spam"
│  └─ Check: SPF/DKIM/DMARC → warm-up → volume → content triggers → domain age
│
└─ "Don't know what's wrong"
   └─ Run full audit checklist above, layer by layer
```
