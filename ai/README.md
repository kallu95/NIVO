# NIVO answer bank

318 questions with model answers, written for expert review.

- `nivo_qa_bank.jsonl` / `.csv`: every item. `type` is `core` (133 hand-written answers on PMS, funds, fees, IPS, behaviour, tax, regulation, execution and NIVO) or `data` (185 answers generated from APMI and AMFI data, with `data_as_of`).
- `../qa.json`: the core answers the app loads. NIVO's offline assistant answers from them, and the AI assistant receives the closest matches as house answers to stay consistent with.

How to use it:
1. Review: experts mark `review_status` as Approved or Needs change and add notes.
2. Evaluate: run every question through NIVO's AI before each release and compare with the approved answer.
3. Fine-tune later: only approved, expert-checked answers.

Data answers go stale: regenerate them after each data refresh. Tax answers deliberately avoid rates; confirm current rules before publishing any.
