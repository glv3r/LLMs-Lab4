SUMMARY_PROMPT_V1 = "Summarize this: "



SUMMARY_SYSTEM_PROMPT_V2 = "You are an assistant to a microfinance loan officer who has a lot of letters " \
"for loan application. CONSTRAINTS: factual, neutral, no invented details, 3-4 sentences"



EXTRACT_PROMPT = "You are to carefully examine the prompt the user has given and return ONLY a JSON object with exactly these keys:" \
"applicant_name: string, amount_ghs: number, purpose: string, monthly_profit_ghs: number or null, " \
"has_collateral_or_guarantor: boolean, and repayment_months: number or null. If a field is not stated in the letter, use " \
"null as instructed. DO NOT GUESS."




BRIEF_PROMPT="You're going to be given two items, a letter, and a JSON block that has information about that letter. You're " \
"going to then use that to give me these things: " \
"1. Strengths (in bullet points, directly from the letter), " \
"2. Risks/Red flags (also in bullet points), " \
"3. Missing information the officer the letter was sent to should request from that user " \
"4. Then suggest the next steps after reviewing the letter e.g. 'invite for interview', 'request documents', 'flag for senior review' — NOT 'approve' or 'reject'. Be specific." \
"Note well that the final decision is made by the human (the officer). You're just an assistant to them, more of a helper if you will."