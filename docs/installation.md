# 📦 Installation Guide

Agent Factory can be installed in multiple ways depending on your preference and setup.

---

## 📋 Requirements

### Mandatory
- **Claude Code**: v4.0 or later
- **Git**: For version control (optional but recommended)

### Optional
- **Context7 MCP**: For official documentation research (recommended)
- **MoAI-ADK**: For enhanced skills integration (optional)

---

## 🚀 Installation Methods

### Method 1: GitHub Direct (Recommended)

The fastest and most straightforward way to install.

```bash
/plugin install https://github.com/GoosLab/claude-code-agent-factory.git
```

**Advantages**:
- ✅ Direct installation from source
- ✅ Always latest version
- ✅ Full control over updates

**Verification**:
```bash
/plugin list
# Should show: agent-factory
```

---

### Method 2: GitHub with Specific Version

Install a specific release version.

```bash
/plugin install https://github.com/GoosLab/claude-code-agent-factory.git@v1.0.0
```

**Available Versions**:
- `v1.0.0` - Initial production release (current)

**Advantages**:
- ✅ Reproducible installations
- ✅ Version pinning for stability
- ✅ Easy rollback to previous versions

---

### Method 3: Claude Code Plugins Plus (Coming Soon)

Install from the community marketplace.

```bash
# First, add the marketplace
/plugin marketplace add jeremylongshore/claude-code-plugins-plus

# Then, install the plugin
/plugin install agent-factory
```

**Status**: Pending approval from Plugins Plus maintainers

**Advantages**:
- ✅ Centralized plugin discovery
- ✅ Community reviews
- ✅ Automatic update notifications

---

## ✅ Verification

After installation, verify everything is working:

### Step 1: Check Installation
```bash
/plugin list
```

Expected output should include:
```
✅ agent-factory (v1.0.0)
   Status: Active
```

### Step 2: Test Agent Loading
```bash
Task(
  subagent_type="agent-factory",
  description="Test installation",
  prompt="Create a simple Python formatter agent"
)
```

Expected output:
- Complete agent markdown file
- Generation report
- Validation results

### Step 3: Verify Skills
```bash
Skill("moai-alfred-agent-factory")
```

Should load without errors.

---

## 🔧 Configuration

### Optional: Enable Context7 MCP

For enhanced documentation research:

1. **Check if Context7 is installed**:
   ```bash
   /mcp list
   ```

2. **If not installed, set it up**:
   - Follow Claude Code official MCP documentation
   - Configure in `.claude/mcp.json`

3. **Verify Context7 is available**:
   ```bash
   Task(
     subagent_type="agent-factory",
     prompt="Create an agent with Context7 research"
   )
   ```

### Optional: Enable MoAI-ADK Integration

For full skill ecosystem access:

1. **Install MoAI-ADK** (if not already installed):
   ```bash
   pip install moai-adk
   ```

2. **Initialize in your project**:
   ```bash
   moai-adk init
   ```

3. **Verify integration**:
   - Access to 128+ MoAI skills
   - Enhanced language detection
   - Full TRUST 5 compliance

---

## 🐛 Troubleshooting

### Issue: "Plugin not found"

**Solution 1**: Verify installation
```bash
/plugin list
# If agent-factory not shown, reinstall:
/plugin install https://github.com/GoosLab/claude-code-agent-factory.git
```

**Solution 2**: Check Claude Code version
```bash
/version
# Ensure v4.0 or later
```

---

### Issue: "Skill 'moai-alfred-agent-factory' not found"

**Possible Causes**:
1. Plugin not fully installed
2. Skills not loaded

**Solutions**:
```bash
# Restart Claude Code
# Then try again:
Skill("moai-alfred-agent-factory")
```

---

### Issue: "Context7 MCP unavailable"

**Expected Behavior**:
- Falls back to WebFetch
- Still generates valid agents
- Just without latest documentation research

**To Enable Context7**:
1. Check `.claude/mcp.json` configuration
2. Verify MCP server is running
3. Test with simple research task

---

### Issue: "Generation fails with timeout"

**Possible Causes**:
1. Complex agent (>30 min expected time)
2. Context7 MCP slow response
3. Network issue

**Solutions**:
1. Wait longer for completion
2. Try simpler agent first
3. Check network connectivity
4. Try without Context7:
   ```bash
   Task(
     subagent_type="agent-factory",
     prompt="Simple agent request without research"
   )
   ```

---

## 📊 Supported Platforms

| Platform | Status | Notes |
|----------|--------|-------|
| macOS | ✅ Supported | Fully tested |
| Linux | ✅ Supported | Fully tested |
| Windows | ✅ Supported | Via WSL2 recommended |
| Online Claude Code | ✅ Supported | Full compatibility |

---

## 🔄 Updates

### Check for Updates
```bash
/plugin list
# Shows current version
```

### Update Plugin
```bash
# Uninstall current version
/plugin uninstall agent-factory

# Reinstall latest
/plugin install https://github.com/GoosLab/claude-code-agent-factory.git
```

### Update History
- **v1.0.0** (2025-11-15): Initial release
- **v1.1.0** (Planned): Preview mode + custom templates
- **v1.2.0** (Planned): Multi-agent generation

---

## 🆘 Getting Help

If you encounter issues during installation:

1. **Check Documentation**: [README.md](../README.md)
2. **Review Examples**: [examples.md](../skills/moai-alfred-agent-factory/examples.md)
3. **Report Issue**: [GitHub Issues](https://github.com/GoosLab/claude-code-agent-factory/issues)
4. **Ask Question**: [GitHub Discussions](https://github.com/GoosLab/claude-code-agent-factory/discussions)

---

## ✨ Next Steps

After successful installation:

1. **Read Quick Start**: [Quick Start Guide](quick-start.md)
2. **Generate First Agent**: Follow 5-minute tutorial
3. **Explore Examples**: Check [examples.md](../skills/moai-alfred-agent-factory/examples.md)
4. **Read Full Documentation**: [agent-factory.md](../agents/agent-factory.md)

---

**Installation complete? Let's generate your first agent!** → [Quick Start Guide](quick-start.md)
