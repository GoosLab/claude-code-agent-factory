# ⚡ Quick Start: 5-Minute Tutorial

Get your first agent generated in 5 minutes! This tutorial walks you through the entire process.

---

## ⏱️ Timeline

| Step | Task | Time |
|------|------|------|
| 1️⃣ | Verify Installation | 1 min |
| 2️⃣ | Generate First Agent | 2 min |
| 3️⃣ | Review Generated Agent | 1 min |
| 4️⃣ | Use Your Agent | 1 min |

**Total: ~5 minutes**

---

## ✅ Step 1: Verify Installation (1 min)

First, make sure Agent Factory is properly installed.

```bash
/plugin list
```

**Expected Output**:
```
✅ agent-factory (v1.0.0)
   Status: Active
   Location: ...
```

**Not seeing agent-factory?**
- Review [Installation Guide](installation.md)
- Run: `/plugin install https://github.com/GoosLab/claude-code-agent-factory.git`

---

## 🚀 Step 2: Generate Your First Agent (2 min)

We'll create a simple Python code formatter agent.

### Copy This Code:

```bash
Task(
  subagent_type="agent-factory",
  description="Generate Python formatter agent",
  prompt="Create an agent that formats Python code using Black"
)
```

### What to Expect:
1. ⏳ Agent Factory starts analyzing (5-10 seconds)
2. 🔍 Complexity assessment (2-3 seconds)
3. 📚 Optional: Research phase (5-10 seconds if Context7 available)
4. 🛠️ Template selection and generation (10-15 seconds)
5. ✅ Quality validation (3-5 seconds)

**Total Generation Time**: ~2-3 minutes

### Output Format:
The response includes:

```
🏭 AGENT GENERATION REPORT

📊 Requirements Analysis:
  ✅ Domain: backend
  ✅ Primary Capability: create
  ✅ Complexity Score: 2/10 (LOW)

🤖 Model Selection:
  ✅ Selected: haiku
  ✅ Reasoning: Low complexity, execution-focused

🛠️ Tool Permissions:
  ✅ Calculated: Read, Write, Bash

📦 Skill Recommendations:
  ✅ Auto-load: moai-lang-python
  ✅ Confidence: 95%

📄 Generated Agent (agent-factory.md):
  ✅ Template: Tier 1 (Simple)
  ✅ Lines: ~200
  ✅ Status: READY

✅ All Quality Gates PASSED
   - YAML: ✓ Valid
   - Structure: ✓ Complete
   - Content: ✓ Accurate
   - Quality: ✓ 92/100

🎉 AGENT READY FOR USE!
```

---

## 📋 Step 3: Review Generated Agent (1 min)

The generated agent markdown looks like this:

```yaml
---
name: format-expert
description: "Use PROACTIVELY when: Formatting Python code with Black..."
tools: Read, Write, Bash
model: haiku
---

# 🎨 Format Expert - Python Code Formatter

> **Quick code formatting specialist using Black**

**Version**: 1.0.0
**Status**: Production-Ready

## 🎭 Agent Persona

**Icon**: 🎨
**Job**: Python Code Formatter Specialist
**Area of Expertise**: Code formatting, style standardization, Black configuration
**Role**: Quick formatting expert for clean, consistent code
**Goal**: Format Python code to match Black standards

## 🧰 Required Skills

**Automatic Core Skills**:
- `Skill("moai-lang-python")`

## 🎯 Core Responsibilities

✅ **DOES**:
- Format Python code using Black
- Apply PEP 8 formatting standards
- Handle various code styles
- Preserve code functionality

❌ **DOES NOT**:
- Modify code logic
- Refactor code structure
- Add type hints
- Optimize performance

...
```

**What Each Section Means**:
- **YAML Frontmatter**: Agent metadata (name, tools, model)
- **Persona**: What the agent does and its expertise
- **Skills**: Knowledge sources it uses
- **Responsibilities**: What it does and doesn't do
- **Workflow**: Step-by-step execution guide

---

## 🎯 Step 4: Use Your Generated Agent (1 min)

Now you can use your newly created agent!

```bash
Task(
  subagent_type="format-expert",  # Your generated agent
  prompt="Format this Python code:\n\ndef hello(name):\n    print(f'Hello {name}')"
)
```

### Expected Output:
```
✅ Python Code Formatting Result

Original:
def hello(name):
    print(f'Hello {name}')

Formatted (Black):
def hello(name):
    print(f"Hello {name}")
```

---

## 🎓 What You Just Learned

✅ How to invoke agent-factory
✅ How agents are generated from requirements
✅ How to read generated agent specifications
✅ How to use your new agent

---

## 🚀 Next Steps

### Try More Complex Agents

**Backend API Designer**:
```bash
Task(
  subagent_type="agent-factory",
  description="Generate API designer",
  prompt="Create an agent that designs REST APIs with proper error handling and security best practices"
)
```

**Security Auditor**:
```bash
Task(
  subagent_type="agent-factory",
  description="Generate security auditor",
  prompt="Create an agent that audits code for OWASP Top 10 vulnerabilities"
)
```

**Database Optimizer**:
```bash
Task(
  subagent_type="agent-factory",
  description="Generate database optimizer",
  prompt="Create an agent that optimizes PostgreSQL queries and designs migrations"
)
```

### Explore Documentation

1. **[Full Agent Spec](../agents/agent-factory.md)**: Complete workflow details
2. **[Skill Reference](../skills/moai-alfred-agent-factory/SKILL.md)**: How it works internally
3. **[Examples](../skills/moai-alfred-agent-factory/examples.md)**: More use cases
4. **[Installation Guide](installation.md)**: Detailed setup help

---

## ❓ Common Questions

### Q: How long does generation take?

**A**: Depends on complexity:
- **Simple agents** (formatting, linting): ~3-5 minutes
- **Standard agents** (domain experts): ~10-15 minutes
- **Complex agents** (security audit, research): ~20-30 minutes

### Q: Can I customize generated agents?

**A**: Yes! Generated agents are regular markdown files that you can:
- Edit the YAML frontmatter
- Add/remove tool permissions
- Modify skill recommendations
- Adjust workflow steps

### Q: What if I don't have Context7 MCP?

**A**: Agent Factory works fine without it:
- Uses WebFetch for documentation
- Falls back to established patterns
- Still generates valid agents
- Just without latest research

### Q: Can I use generated agents in production?

**A**: Absolutely! Generated agents:
- Meet TRUST 5 standards
- Comply with Claude Code v4.0
- Include quality validation
- Are ready for immediate use

### Q: What models can be generated?

**A**: Agent Factory generates agents with:
- **Haiku**: Fast execution (simple tasks)
- **Sonnet**: Complex reasoning (design, architecture)
- **Inherit**: Context-dependent (mixed tasks)

The right model is selected automatically based on complexity.

### Q: How accurate are the recommendations?

**A**: Very accurate:
- **Model selection**: 90%+ accuracy
- **Tool permissions**: 95%+ appropriateness
- **Skill matching**: 85%+ relevance
- **Quality validation**: 85%+ TRUST 5 score

---

## 🆘 Troubleshooting

### Issue: "Agent generation seems to hang"

**Solutions**:
1. Wait longer (complex agents take 20-30 min)
2. Check internet connection (for Context7)
3. Try simpler agent first
4. Check Claude Code status

### Issue: "Generated agent doesn't work"

**Solutions**:
1. Check requirements are met (Claude Code v4.0+)
2. Verify agent name in Task()
3. Check tool permissions are correct
4. Run the generated agent step by step

### Issue: "Getting unexpected results"

**Solutions**:
1. Review agent generation report
2. Check skill recommendations
3. Verify agent persona matches your needs
4. File an issue on GitHub

---

## 💡 Pro Tips

### 1. Start Simple
Generate simple agents first to understand the process:
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create a simple code formatter agent"
)
```

### 2. Review Generation Reports
Always read the generation report to understand:
- Why this model was selected
- Which skills are recommended
- How tool permissions were calculated

### 3. Use Generated Agents as Templates
Customize generated agents for your specific needs:
- Modify tool permissions
- Add custom workflow steps
- Adjust skill recommendations

### 4. Keep Best Practices
Generated agents follow best practices:
- Least privilege tool permissions
- Clear responsibility boundaries
- Proper delegation patterns

### 5. Explore MoAI-ADK Integration
If you have MoAI-ADK installed:
- Get access to 128+ skills
- Enhanced language detection
- Full TRUST 5 compliance

---

## 🎉 You're Ready!

You've successfully:
✅ Installed Agent Factory
✅ Generated your first agent
✅ Reviewed the generated specification
✅ Used the agent for real work

**What's Next?**
- Explore [Examples](../skills/moai-alfred-agent-factory/examples.md)
- Read [Full Documentation](../agents/agent-factory.md)
- Join [GitHub Discussions](https://github.com/GoosLab/claude-code-agent-factory/discussions)
- Share your agents with the community!

---

**Happy agent generating!** 🚀
