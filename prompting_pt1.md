**Credits to: [Orginal Post](https://www.reddit.com/r/PromptEngineering/s/PvHwfBau5x)**

AI Prompting (1/10): Essential Foundation Techniques Everyone Should Know

```markdown
 ┌─────────────────────────────────────────────────────┐
    ◆ 𝙿𝚁𝙾𝙼𝙿𝚃 𝙴𝙽𝙶𝙸𝙽𝙴𝙴𝚁𝙸𝙽𝙶: 𝙵𝙾𝚄𝙽𝙳𝙰𝚃𝙸𝙾𝙽 𝚃𝙴𝙲𝙷𝙽𝙸𝚀𝚄𝙴𝚂    
                     【１/１０】                      
 └─────────────────────────────────────────────────────┘
```
**TL;DR:** Learn how to craft prompts that go beyond basic instructions. We'll cover role-based prompting, system message optimization, and prompt structures with real examples you can use today.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

## ◈ 1. Beyond Basic Instructions

Gone are the days of simple "Write a story about..." prompts. Modern prompt engineering is about creating structured, context-rich instructions that consistently produce high-quality outputs. Let's dive into what makes a prompt truly effective.

### ◇ Key Components of Advanced Prompts:
```markdown
1. Role Definition
2. Context Setting
3. Task Specification
4. Output Format
5. Quality Parameters
```
## ◆ 2. Role-Based Prompting

One of the most powerful techniques is role-based prompting. Instead of just requesting information, you define a specific role for the AI.

### ❖ Basic vs Advanced Approach:
```markdown
**Basic Prompt:**
Write a technical analysis of cloud computing.
```
**Advanced Role-Based Prompt:**
```markdown
As a Senior Cloud Architecture Consultant with 15 years of experience:
1. Analyses the current state of cloud computing
2. Focus on enterprise architecture implications
3. Highlight emerging trends and their impact
4. Present your analysis in a professional report format
5. Include specific examples from major cloud providers
```
### ◎ Why It Works Better:
- Provides clear context
- Sets expertise level
- Establishes consistent voice
- Creates structured output
- Enables deeper analysis

## ◈ 3. Context Layering

Advanced prompts use multiple layers of context to enhance output quality.

### ◇ Example of Context Layering:
```markdown
CONTEXT: Enterprise software migration project
AUDIENCE: C-level executives
CURRENT SITUATION: Legacy system reaching end-of-life
CONSTRAINTS: 6-month timeline, $500K budget
REQUIRED OUTPUT: Strategic recommendation report

Based on this context, provide a detailed analysis of...
```
## ◆ 4. Output Control Through Format Specification

### ❖ Template Technique:
```markdown
Please structure your response using this template:

[Executive Summary]
- Key points in bullet form
- Maximum 3 bullets

[Detailed Analysis]
1. Current State
2. Challenges
3. Opportunities

[Recommendations]
- Prioritized list
- Include timeline
- Resource requirements

[Next Steps]
- Immediate actions
- Long-term considerations
```
## ◈ 5. Practical Examples

Let's look at a complete advanced prompt structure:
```markdown
ROLE: Senior Systems Architecture Consultant
TASK: Legacy System Migration Analysis

CONTEXT:
- Fortune 500 retail company
- Current system: 15-year-old monolithic application
- 500+ daily users
- 99.99% uptime requirement

REQUIRED ANALYSIS:
1. Migration risks and mitigation strategies
2. Cloud vs hybrid options
3. Cost-benefit analysis
4. Implementation roadmap

OUTPUT FORMAT:
- Executive brief (250 words)
- Technical details (500 words)
- Risk matrix
- Timeline visualization
- Budget breakdown

CONSTRAINTS:
- Must maintain operational continuity
- Compliance with GDPR and CCPA
- Maximum 18-month implementation window
```
## ◆ 6. Common Pitfalls to Avoid

1. **Over-specification**
   - Too many constraints can limit creative solutions
   - Find balance between guidance and flexibility

2. **Under-contextualization**
   - Not providing enough background
   - Missing critical constraints

3. **Inconsistent Role Definition**
   - Mixing expertise levels
   - Conflicting perspectives

## ◈ 7. Advanced Tips

1. **Chain of Relevance:**
   - Connect each prompt element logically
   - Ensure consistency between role and expertise level
   - Match output format to audience needs

2. **Validation Elements:**
```markdown
   VALIDATION CRITERIA:
   - Must include quantifiable metrics
   - Reference industry standards
   - Provide actionable recommendations
```
## ◆ 8. Next Steps in the Series

Next post will cover "Chain-of-Thought and Reasoning Techniques," where we'll explore making AI's thinking process more explicit and reliable. We'll examine:
- Zero-shot vs Few-shot CoT
- Step-by-step reasoning strategies
- Advanced reasoning frameworks
- Output validation techniques

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

*𝙴𝚍𝚒𝚝: If you found this helpful, check out my profile for more posts in this series on Prompt Engineering.*
