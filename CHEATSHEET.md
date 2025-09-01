# AI-Native Dev Cheatsheet

Using AI-integrated development tools like Cursor, Aider, or GitHub Copilot can improve productivity on suitable tasks. This comprehensive cheatsheet provides honest assessments across all common development tasks.

**Results vary significantly** based on experience, codebase, team dynamics, and domain.

---

## ⚠️ Critical Warnings First

### For Junior Developers (0-3 years experience)
**Use AI tools sparingly.** Extensive use early in your career can severely impact:
- Problem-solving skill development
- Debugging ability
- Understanding of fundamentals
- Technical interview performance
- Ability to work without AI tools

### Security & Compliance - NEVER Use AI For:
- Authentication/authorization implementation
- Cryptographic implementations or security algorithms
- Payment processing logic
- HIPAA/PCI/SOC2 compliance code
- Password handling or encryption keys
- Random number generation for security
- Database transaction handling
- Financial calculations
- Production incident response

---

## Prerequisites for Success

Before adopting AI tools, ensure you have:
- [ ] Strong code review culture
- [ ] Established coding standards
- [ ] Security review process in place
- [ ] Team agreement on AI usage guidelines
- [ ] Understanding of data privacy implications
- [ ] Plan to maintain and practice core skills

**Without these prerequisites, AI integration may decrease code quality.**

---

## Comprehensive Task Assessment

### 🟢 High-Value Tasks (30-60% potential time savings)

#### Core Development
| Task | Traditional | With AI | Key Consideration |
|------|-------------|---------|-------------------|
| **Unit Test Generation** | 30-45 min | 10-20 min | Verify tests actually test functionality |
| **Documentation** | 30 min | 8-15 min | Add human context for "why" |
| **Boilerplate/CRUD** | 45-60 min | 15-25 min | Watch for pattern drift |
| **Mock Data** | 30 min | 2-5 min | Best AI use case |
| **Regular Expressions** | 15-20 min | 3-5 min | Test edge cases thoroughly |
| **TypeScript Types** | 20-30 min | 5-10 min | Review for accuracy |
| **Validation Schemas** | 20-25 min | 5-10 min | Zod/Yup generation works well |

#### API & Documentation
| Task | Traditional | With AI | Key Consideration |
|------|-------------|---------|-------------------|
| **OpenAPI/Swagger Specs** | 40 min | 10-15 min | From existing code |
| **Postman Collections** | 30 min | 5-10 min | From API specs |
| **API Client Generation** | 45 min | 15-20 min | From OpenAPI specs |
| **README Files** | 30 min | 8-12 min | Structure and basics |

#### DevOps & Configuration
| Task | Traditional | With AI | Key Consideration |
|------|-------------|---------|-------------------|
| **Basic Dockerfiles** | 20 min | 5-8 min | Standard patterns only |
| **CI/CD Configs** | 60 min | 20-30 min | GitHub Actions, Jenkins |
| **Environment Configs** | 20 min | 8-10 min | .env templates |

### 🟡 Moderate-Value Tasks (15-30% potential time savings)

#### Backend Development
| Task | Traditional | With AI | Why Moderate |
|------|-------------|---------|--------------|
| **SQL Queries** | 25 min | 15-20 min | Need optimization |
| **Database Migrations** | 30 min | 20-25 min | Need careful review |
| **GraphQL Schemas** | 30 min | 20 min | Resolvers need customization |
| **Background Workers** | 40 min | 25-30 min | Queue-specific logic |
| **ETL Pipelines** | 45 min | 30 min | Business logic heavy |
| **Batch Processing** | 35 min | 25 min | Performance considerations |

#### Frontend Development
| Task | Traditional | With AI | Why Moderate |
|------|-------------|---------|--------------|
| **Component Scaffolding** | 15 min | 8-12 min | Team patterns vary |
| **CSS/Styling** | 20 min | 12-15 min | Design system specific |
| **Form Validation** | 25 min | 15-20 min | UX requirements vary |
| **State Management** | 30 min | 20 min | Architecture dependent |

#### Infrastructure & DevOps
| Task | Traditional | With AI | Why Moderate |
|------|-------------|---------|--------------|
| **Terraform/IaC** | 45 min | 30 min | Environment specific |
| **Kubernetes Manifests** | 40 min | 25-30 min | Cluster specific |
| **Ansible Playbooks** | 35 min | 25 min | Infrastructure dependent |
| **Monitoring Configs** | 30 min | 20 min | Metric understanding needed |

#### Testing
| Task | Traditional | With AI | Why Moderate |
|------|-------------|---------|--------------|
| **Integration Tests** | 40 min | 25-30 min | Complex scenarios |
| **E2E Tests** | 60 min | 40 min | Flow understanding needed |
| **Contract Tests** | 30 min | 20 min | API specifics |

### 🔴 Low-Value or Risky Tasks (0-15% savings or negative)

#### Should Approach with Caution
| Task | Why Limited/Risky | Better Approach |
|------|------------------|-----------------|
| **Performance Tests** | Needs real metrics | Use profiling tools |
| **Caching Strategies** | Needs traffic patterns | Measure first |
| **Database Indexing** | Needs query analysis | Use EXPLAIN plans |
| **Rate Limiting** | Needs threat model | Security review |
| **Complex Debugging** | Can mislead | Use debugger |
| **Architecture Design** | Lacks context | Team discussion |
| **Accessibility Fixes** | Compliance risk | Use a11y tools |
| **Security Headers** | High risk if wrong | Security checklist |

#### Often Slower with AI
| Task | Why | Alternative |
|------|-----|------------|
| **Commit Messages** | Edit time > write time | Write directly |
| **Code Review Comments** | Needs human insight | Personal feedback |
| **PR Descriptions** | Missing context | Manual writing |
| **Import Organization** | IDEs do this better | Use IDE features |
| **Variable Naming** | Context dependent | Think it through |

### ❌ Never Use AI For

#### Security & Compliance
- Authentication/authorization logic
- Encryption/cryptography
- Payment processing
- Compliance code (HIPAA, PCI, GDPR)
- Security-critical validation
- Session management
- Token generation

#### Critical Systems
- Database transactions
- Concurrent programming
- Memory management
- Financial calculations
- Production debugging
- Incident response
- Error recovery logic

---

## Task-Specific Guidance

### Frontend Tasks
```markdown
✅ Good for AI:
- Component boilerplate
- Basic form validation
- Mock data generation
- Test generation

⚠️ Review Carefully:
- State management setup
- Performance optimizations
- Accessibility implementation
- Animation logic

❌ Avoid AI:
- Security-related code
- Payment UI logic
- Complex business logic
```

### Backend Tasks
```markdown
✅ Good for AI:
- CRUD endpoints
- Basic validations
- Database seeders
- API documentation

⚠️ Review Carefully:
- Background job logic
- Caching implementation
- Rate limiting
- Database queries

❌ Avoid AI:
- Authentication
- Transaction handling
- Financial logic
```

### DevOps Tasks
```markdown
✅ Good for AI:
- Basic Docker configs
- CI/CD templates
- Environment setup
- Documentation

⚠️ Review Carefully:
- Infrastructure as Code
- Monitoring setup
- Deployment scripts
- Security configs

❌ Avoid AI:
- Production secrets
- Security policies
- Compliance configs
```

### Mobile Development
```markdown
✅ Good for AI:
- Component scaffolding
- Basic layouts
- Test generation
- App store descriptions

⚠️ Review Carefully:
- Platform-specific code
- Push notifications
- Deep linking
- Background tasks

❌ Avoid AI:
- In-app purchases
- Security storage
- Biometric auth
```

### Data Engineering
```markdown
✅ Good for AI:
- SQL queries (review performance)
- ETL pipeline structure
- Data validation scripts
- Report templates

⚠️ Review Carefully:
- Data transformations
- Aggregation logic
- Migration scripts
- Batch processing

❌ Avoid AI:
- PII handling
- Compliance logic
- Financial calculations
```

---

## Realistic Workflow by Task Type

### For Boilerplate Tasks
```
1. Generate with AI (2 min)
2. Review for patterns (1 min)
3. Adjust to standards (2 min)
Total: 5 min vs 15 min manual
```

### For Complex Logic
```
1. Generate with AI (2 min)
2. Review carefully (5 min)
3. Fix issues (5 min)
4. Debug problems (10 min)
Total: 22 min vs 20 min manual (negative value!)
```

### For Tests
```
1. Generate test suite (2 min)
2. Review for coverage (3 min)
3. Add missing cases (5 min)
4. Verify they work (5 min)
Total: 15 min vs 30 min manual
```

---

## Domain-Specific Considerations

### Web Development
- **High value:** Component generation, tests, docs
- **Medium value:** State management, API integration
- **Low value:** Performance optimization, SEO

### Systems Programming
- **High value:** Documentation, basic tests
- **Medium value:** Boilerplate code
- **Avoid:** Memory management, concurrency

### Data Engineering
- **High value:** SQL generation, documentation
- **Medium value:** ETL pipelines, validations
- **Avoid:** Financial calculations, PII handling

### DevOps/SRE
- **High value:** Config templates, runbooks
- **Medium value:** IaC, monitoring setup
- **Avoid:** Security policies, incident response

### Mobile Development
- **High value:** UI components, layouts
- **Medium value:** Navigation, state
- **Avoid:** Platform-specific optimizations

---

## Quick Reference by Scenario

### "I need this done fast"
✅ Use AI for:
- Boilerplate
- Mock data
- Basic tests
- Documentation templates

### "This is business-critical"
❌ Don't use AI for:
- Core business logic
- Financial calculations
- Security features
- Performance-critical code

### "I'm learning this technology"
⚠️ Limited AI use:
- See examples
- Understand patterns
- But write code manually

### "This is for production"
Review everything:
- Security implications
- Performance impact
- Error handling
- Edge cases

---

## The Bottom Line

AI tools can help with **mechanical, pattern-based tasks** where:
- The pattern is well-established
- Errors are easy to catch
- Security isn't critical
- Performance isn't critical

They struggle with **complex, context-dependent tasks** that need:
- Deep domain knowledge
- Security considerations
- Performance optimization
- Business logic understanding

**Success requires:**
- Knowing which is which
- Reviewing everything
- Maintaining your skills
- Realistic expectations

---

> AI tools are amplifiers, not replacements.
> They amplify both good and bad practices.
> Use them where they demonstrably help.
> Skip them where they don't.
> Always maintain your fundamental skills.
