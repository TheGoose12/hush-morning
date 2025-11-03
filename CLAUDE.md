# Claude Code Assistant Rules & Shortcuts

## 🚨 **CRITICAL: File Protection Protocol - NEVER DELETE CORE FILES**


### **MANDATORY File Modification Protocol:**

#### **Before ANY Destructive Changes:**
- **Read the ENTIRE file first** using Read tool to understand scope and complexity

---

## 🧪 **CRITICAL: Testing Protocol **
Before telling me anything is done, you need to use Playwright or Puppeteer to test.

#### **Automated Testing :**
Before confirming that any feature is working perfectly, complete, or good to go, you will test that the feature is working with Playwright or Puppeteer. 


---

## Project Quick Commands

### Context & Onboarding
- **`-q new`** → Read project context and README files for new developers/sessions
- **`-q context`** → Read all project documentation (context, architecture, best practices)
- **`-q overview`** → Quick project overview and current state
- **`-q help`** → Show all available shortcuts and commands
- **`-shortcuts`** → Quick reference list of all custom shortcuts
- **`-q plan`** → Execute consistency check before implementing new features

## -q plan (Query Plan for Consistency)

Before implementing any new feature or significant change, execute a -q plan to ensure consistency and efficiency:

### The -q Plan Process:

1. **Query Similar Patterns**
   - Search for similar functionality in the codebase
   - Identify at least 2-3 examples of related implementations
   - Note the patterns, components, and structures used

2. **Question the Approach**
   - Is this consistent with existing patterns?
   - Can we reuse or extend existing components?
   - Are we using our centralized CSS and established utilities?
   - What's the minimal code needed?

3. **Qualify the Solution**
   - Verify alignment with our architecture
   - Confirm no duplication of existing functionality
   - Ensure we're following established data flow patterns
   - Check that new code matches the style of similar features

### When to Use -q plan:
- Adding new components or features
- Modifying existing functionality
- Creating new data visualizations
- Adding new pages or sections
- Implementing new interactions

### Example Output:
```
-q plan: Adding monthly revenue chart

Query: Found similar charts in Overview (line chart), Growth Ramp (projection chart)
Question: Can reuse BaseChart component with revenue data props
Qualify: Will follow same pattern as Growth Summary chart, use existing chart utilities
Conclusion: Extend BaseChart, 15 lines of new code vs 200 for custom implementation
```

### Key Principle:
**Consistency > Innovation** - The codebase should feel cohesive. Always prefer extending existing patterns over creating new ones.

### Development Commands
- **`-d analyze`** → Analyze codebase structure and dependencies
- **`-d test`** → Run all tests and show results
- **`-d lint`** → Run linting and type checking
- **`-d build`** → Build the project and check for errors
- **`-d hot`** → Enable/disable hot reload for development

### Feature Development
- **`-f overview`** → Focus on Overview tab features and functionality
- **`-f funnel`** → Focus on Funnel view features
- **`-f config`** → Work on configuration panel features
- **`-f ui`** → Focus on UI/UX improvements
- **`-f bug`** → Bug fix mode - analyze and fix issues

### Code Review & Quality
- **`-r code`** → Review recent changes and code quality
- **`-r performance`** → Analyze performance and optimization opportunities
- **`-r architecture`** → Review overall architecture and patterns
- **`-r security`** → Security review and best practices check

### Project Management
- **`-p status`** → Current project status and version info
- **`-p todo`** → Show pending tasks and improvements
- **`-p deploy`** → Deployment checklist and verification
- **`-p clean`** → Clean up temp files and optimize project

## Auto-Actions for Common Shortcuts

When you see these patterns, automatically:

### `-q new` Action Sequence:
1. Read `/Users/ronsparks/Desktop/claudeMake/hush-scout-v2/project-context.md`
2. Read `/Users/ronsparks/Desktop/claudeMake/hush-scout-v2/COMPONENT-ARCHITECTURE-README.md`
3. Read `/Users/ronsparks/Desktop/claudeMake/hush-scout-v2/development-best-practices.md`
4. Provide concise project summary and current capabilities

### `-d test` Action Sequence:
1. Look for test commands in package.json or project files
2. Run available tests
3. Report results and any failures
4. Suggest fixes for failing tests

### `-f overview` Action Sequence:
1. Read `/Users/ronsparks/Desktop/claudeMake/hush-scout-v2/sections/analytics/overview.html`
2. Read related CSS and JS files
3. Ready to work on Overview tab features

### `-p status` Action Sequence:
1. Check git status and recent commits
2. Show current version (check index.html for version number)
3. List recent changes and current branch
4. Report any uncommitted changes

## Project-Specific Context

### Key Files to Always Consider:
- **Main App:** `/Users/ronsparks/Desktop/claudeMake/hush-scout-v2/index.html`
- **Navigation:** `/Users/ronsparks/Desktop/claudeMake/hush-scout-v2/assets/js/navigation.js`
- **Data Management:** `/Users/ronsparks/Desktop/claudeMake/hush-scout-v2/data/dataManager.js`
- **Analytics:** `/Users/ronsparks/Desktop/claudeMake/hush-scout-v2/sections/analytics/analytics.js`

### Current Version System:
- Version number located in `index.html` around line 1412: `<span class="version-number">v.XXX</span>`
- Increment version number for any feature updates
- Current version: v.115 (as of last update)

### Development Patterns:
- Use existing `dataManager.js` for all data persistence
- Follow Smart Value link patterns for interactive elements
- Maintain collapsible/reorderable section functionality
- Preserve user preferences across sessions

### Common Tasks:
- **Feature updates:** Always increment version number
- **Testing:** Use browser at `http://localhost:8000`
- **Configuration:** Use configuration panel in Analytics section
- **Persistence:** Integrate with `window.dataManager.data` structure

## Quick Reference Commands

**Most Common:**
- `-q new` - Start here for any new session
- `-f overview` - Work on main dashboard
- `-d test` - Verify everything works
- `-p status` - Check current state

**Development:**
- `-d analyze` - Understand code structure
- `-f ui` - Improve user experience
- `-r code` - Review and cleanup

**Project Management:**
- `-p todo` - See what needs work
- `-p deploy` - Ready for deployment
- `-p clean` - Cleanup and optimize

Remember to increment version numbers and test changes at `http://localhost:8000`

---

## -shortcuts (Quick Reference)

### 🔍 **Query Commands**
| Command | Action |
|---------|--------|
| `-q new` | Read project context for new developers/sessions |
| `-q context` | Read all project documentation |
| `-q overview` | Quick project overview and current state |
| `-q help` | Show all available shortcuts and commands |
| `-q plan` | Execute consistency check before implementing features |

### ⚙️ **Development Commands**  
| Command | Action |
|---------|--------|
| `-d analyze` | Analyze codebase structure and dependencies |
| `-d test` | Run all tests and show results |
| `-d lint` | Run linting and type checking |
| `-d build` | Build project and check for errors |
| `-d hot` | Enable/disable hot reload for development |

### 🎨 **Feature Commands**
| Command | Action |
|---------|--------|
| `-f overview` | Focus on Overview tab features and functionality |
| `-f funnel` | Focus on Funnel view features |
| `-f config` | Work on configuration panel features |
| `-f ui` | Focus on UI/UX improvements |
| `-f bug` | Bug fix mode - analyze and fix issues |

### 👁️ **Review Commands**
| Command | Action |
|---------|--------|
| `-r code` | Review recent changes and code quality |
| `-r performance` | Analyze performance and optimization opportunities |
| `-r architecture` | Review overall architecture and patterns |
| `-r security` | Security review and best practices check |

### 📋 **Project Commands**
| Command | Action |
|---------|--------|
| `-p status` | Current project status and version info |
| `-p todo` | Show pending tasks and improvements |
| `-p deploy` | Deployment checklist and verification |
| `-p clean` | Clean up temp files and optimize project |

### 📖 **Meta Commands**
| Command | Action |
|---------|--------|
| `-shortcuts` | Show this quick reference table |
| `-q help` | Detailed help and usage examples |

**💡 Pro Tip:** Always use `-q plan` before significant changes to maintain consistency!

---
