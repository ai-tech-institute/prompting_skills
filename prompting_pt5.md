**Credits to: [Original Post](https://www.reddit.com/r/PromptEngineering/s/Jck8B1N7JR)**

# AI Prompting (5/10): Hallucination Prevention & Error Recovery—Techniques Everyone Should Know

```markdown
┌─────────────────────────────────────────────────────┐
        ◆ 𝙿𝚁𝙾𝙼𝙿𝚃 𝙴𝙽𝙶𝙸𝙽𝙴𝙴𝚁𝙸𝙽𝙶: 𝙴𝚁𝚁𝙾𝚁 𝙷𝙰𝙽𝙳𝙻𝙸𝙽𝙶       
                     【５/１０】                      
└─────────────────────────────────────────────────────┘
```
**TL;DR:** Learn how to prevent, detect, and handle AI errors effectively. Master techniques for maintaining accuracy and recovering from mistakes in AI responses.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## ◈ 1. Understanding AI Errors

AI can make several types of mistakes. Understanding these helps us prevent and handle them better.

### ◇ Common Error Types:
- Hallucination (making up facts)
- Context confusion
- Format inconsistencies
- Logical errors
- Incomplete responses

## ◆ 2. Error Prevention Techniques

The best way to handle errors is to prevent them. Here's how:

**Basic Prompt (Error-Prone):**
```markdown
Summarize the company's performance last year.
```

**Error-Prevention Prompt:**
```markdown
Provide a summary of the company's 2024 performance using these constraints:

SCOPE:
- Focus only on verified financial metrics
- Include specific quarter-by-quarter data
- Reference actual reported numbers

REQUIRED VALIDATION:
- If a number is estimated, mark with "Est."
- If data is incomplete, note which periods are missing
- For projections, clearly label as "Projected"

FORMAT:
Metric: [Revenue/Profit/Growth]
Q1-Q4 Data: [Quarterly figures]
YoY Change: [Percentage]
Data Status: [Verified/Estimated/Projected]
```

### ❖ Why This Works Better:
- Clearly separates verified and estimated data
- Prevents mixing of actual and projected numbers
- Makes any data gaps obvious
- Ensures transparent reporting

## ◈ 3. Self-Verification Techniques

Get AI to check its own work and flag potential issues.

**Basic Analysis Request:**
```markdown
Analyze this sales data and give me the trends.
```

**Self-Verifying Analysis Request:**
```markdown
Analyse this sales data using this verification framework:

1. Data Check
   - Confirm data completeness
   - Note any gaps or anomalies
   - Flag suspicious patterns

2. Analysis Steps
   - Show your calculations
   - Explain methodology
   - List assumptions made

3. Results Verification
   - Cross-check calculations
   - Compare against benchmarks
   - Flag any unusual findings

4. Confidence Level
   - High: Clear data, verified calculations
   - Medium: Some assumptions made
   - Low: Significant uncertainty

FORMAT RESULTS AS:
Raw Data Status: [Complete/Incomplete]
Analysis Method: [Description]
Findings: [List]
Confidence: [Level]
Verification Notes: [Any concerns]
```

## ◆ 4. Error Detection Patterns

Learn to spot potential errors before they cause problems.

### ◇ Inconsistency Detection:
```markdown
VERIFY FOR CONSISTENCY:
1. Numerical Checks
   - Do the numbers add up?
   - Are percentages logical?
   - Are trends consistent?

2. Logical Checks
   - Are conclusions supported by data?
   - Are there contradictions?
   - Is the reasoning sound?

3. Context Checks
   - Does this match known facts?
   - Are references accurate?
   - Is timing logical?
```

### ❖ Hallucination Prevention:
```markdown
FACT VERIFICATION REQUIRED:
- Mark speculative content clearly
- Include confidence levels
- Separate facts from interpretations
- Note information sources
- Flag assumptions explicitly
```

## ◈ 5. Error Recovery Strategies

When you spot an error in AI's response, here's how to get it corrected:

**Error Correction Prompt:**
```markdown
In your previous response about [topic], there was an error:
[Paste the specific error or problematic part]

Please:
1. Correct this specific error
2. Explain why it was incorrect
3. Provide the correct information
4. Note if this error affects other parts of your response
```

**Example:**
```markdown
In your previous response about our Q4 sales analysis, 
you stated our growth was 25% when comparing Q4 to Q3. 
This is incorrect as per our financial reports.

Please:
1. Correct this specific error
2. Explain why it was incorrect
3. Provide the correct Q4 vs Q3 growth figure
4. Note if this affects your other conclusions
```

## ◆ 6. Format Error Prevention

Prevent format-related errors with clear templates:

**Template Enforcement:**
```markdown
OUTPUT REQUIREMENTS:
1. Structure
   [ ] Section headers present
   [ ] Correct nesting levels
   [ ] Consistent formatting

2. Content Checks
   [ ] All sections completed
   [ ] Required elements present
   [ ] No placeholder text

3. Format Validation
   [ ] Correct bullet usage
   [ ] Proper numbering
   [ ] Consistent spacing
```

## ◈ 7. Logic Error Prevention

Here's how to ask AI to verify its own logical reasoning:

```markdown
Before providing your final answer about [topic], please verify your reasoning using these steps:

1. Check Your Starting Point
   "I based my analysis on these assumptions..."
   "I used these definitions..."
   "My starting conditions were..."

2. Verify Your Reasoning Steps
   "Here's how I reached my conclusion..."
   "The key steps in my reasoning were..."
   "I moved from A to B because..."

3. Validate Your Conclusions
   "My conclusion follows from the steps because..."
   "I considered these alternatives..."
   "These are the limitations of my analysis..."
```

**Example:**
```markdown
Before providing your final recommendation for our marketing strategy, please:

1. State your starting assumptions about:
   - Our target market
   - Our budget
   - Our timeline

2. Show how you reached your recommendation by:
   - Explaining each step
   - Showing why each decision leads to the next
   - Highlighting key turning points

3. Validate your final recommendation by:
   - Connecting it back to our goals
   - Noting any limitations
   - Mentioning alternative approaches considered
```

## ◆ 8. Implementation Guidelines

1. **Always Include Verification Steps**
   - Build checks into initial prompts
   - Request explicit uncertainty marking
   - Include confidence levels

2. **Use Clear Error Categories**
   - Factual errors
   - Logical errors
   - Format errors
   - Completion errors

3. **Maintain Error Logs**
   - Track common issues
   - Document successful fixes
   - Build prevention strategies

## ◈ 9. Next Steps in the Series

Our next post will cover "Prompt Engineering: Task Decomposition Techniques (6/10)," where we'll explore:
- Breaking down complex tasks
- Managing multi-step processes
- Ensuring task completion
- Quality control across steps

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

*𝙴𝚍𝚒𝚝: If you found this helpful, check out my profile for more posts in this series on Prompt Engineering....*
