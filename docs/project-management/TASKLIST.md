# coditect-labs-universal-agent-framework - Task List

## Overview

**Repository:** coditect-labs-universal-agent-framework
**Category:** labs/
**Phase:** 1.3
**Current Score:** 80/100
**Target Score:** 90+/100
**Status:** 📋 PLANNED

---

## Quick Status

| Task | Status | Time |
|------|--------|------|
| CLAUDE.md | ⏳ | 30-45 min |
| Symlinks | ⏳ | 15 min |
| Directory Structure | ✅ | 20 min |
| Compliance Check | ⏳ | 15 min |
| Git Sync | ⏳ | 10 min |
| **Total** | ⏳ | ~1-1.5 hours |

---

## Tasks

### Task 1: Refactor CLAUDE.md (300 → <150 lines) (45 min)

- [ ] Analyze current CLAUDE.md (300 lines)
- [ ] Identify content to move to docs/
- [ ] Create docs/ subdirectories as needed
- [ ] Move detailed documentation to docs/
- [ ] Refactor CLAUDE.md to reference docs/
- [ ] Verify <150 lines achieved
- [ ] Commit: 'refactor: Reduce CLAUDE.md to <150 lines'

### Task 2: Verify/Create Symlinks (15 min)

- [ ] .coditect symlink exists → distributed intelligence
- [ ] .claude symlink exists → .coditect
- [ ] Verify symlinks resolve correctly
- [ ] Test: ls -la .coditect .claude

### Task 3: Standardize Directory Structure (20 min)

- [x] docs/ directory exists
- [ ] docs/ has appropriate subdirectories
- [ ] No misplaced files in root
- [ ] .gitignore present and correct
- [ ] README.md present and current

### Task 4: Compliance Verification (15 min)

- [ ] Run compliance analysis script
- [ ] Verify score ≥ 90/100 (current: 80/100)
- [ ] Document any remaining gaps
- [ ] Create remediation plan if needed

### Task 5: Git Sync (10 min)

- [ ] Stage all changes
- [ ] Commit with conventional message
- [ ] Push to remote
- [ ] Notify master orchestrator


---

## Completion Checklist

### Pre-Completion
- [ ] All tasks above marked complete
- [ ] Compliance score verified ≥ 90/100
- [ ] All changes committed and pushed

### Post-Completion
- [ ] Master repo pointer updated
- [ ] Phase status updated in master TASKLIST.md
- [ ] MEMORY-CONTEXT checkpoint created (if significant)

---

## Commands Reference

```bash
# Check compliance score
python3 ../../scripts/analyze-submodule-compliance.py --submodule labs/coditect-labs-universal-agent-framework

# Verify symlinks
ls -la .coditect .claude

# Check CLAUDE.md line count
wc -l CLAUDE.md

# Git sync
git add . && git commit -m "chore: Standardize to CODITECT compliance" && git push

# Update master pointer
cd ../.. && git add submodules/labs/coditect-labs-universal-agent-framework && git commit -m "chore(submodule): Update coditect-labs-universal-agent-framework"
```

---

## Integration

**Master Orchestrator:**
- `docs/project-management/PROJECT-PLAN.md` - Phase 1.3
- `docs/project-management/TASKLIST.md` - Phase 1.3 tasks

**Agents:**
- `project-organizer` - Directory standardization
- `git-workflow-orchestrator` - Sync operations

---

**Last Updated:** 2025-12-09
**Managed By:** CODITECT Orchestrator
