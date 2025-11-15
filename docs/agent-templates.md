# 🏭 Agent Factory - 생성 가능한 에이전트 목록

Agent Factory로 자동 생성할 수 있는 다양한 에이전트들의 예제 목록입니다.

---

## 📋 에이전트 카테고리별 분류

### 1️⃣ 백엔드 개발 (Backend Development)

#### ✅ REST API Designer
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs REST APIs with proper HTTP semantics, error handling, and security best practices"
)
```

**생성될 에이전트**:
- 이름: `rest-api-designer` (또는 유사)
- 모델: Sonnet (아키텍처 설계)
- 스킬: moai-domain-backend, moai-essentials-perf
- 도구: Read, Write, Edit, WebFetch, AskUserQuestion

---

#### ✅ GraphQL API Designer
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs GraphQL APIs with schema design, query optimization, and performance tuning"
)
```

**생성될 에이전트**:
- 이름: `graphql-designer`
- 모델: Sonnet
- 스킬: moai-domain-backend, moai-essentials-perf
- 복잡도: 중간~높음

---

#### ✅ Microservices Architect
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs microservices architecture with domain-driven design, communication patterns, and deployment strategies"
)
```

**생성될 에이전트**:
- 이름: `microservices-architect`
- 모델: Sonnet (복잡한 설계)
- 스킬: moai-domain-backend, moai-domain-devops
- 시간: 20-30분

---

### 2️⃣ 프론트엔드 개발 (Frontend Development)

#### ✅ React Component Builder
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that builds accessible React components with TypeScript, hooks, and state management patterns"
)
```

**생성될 에이전트**:
- 이름: `react-component-builder`
- 모델: Sonnet
- 스킬: moai-lang-typescript, moai-domain-frontend
- 도구: Read, Write, Edit, MultiEdit

---

#### ✅ UI/UX Designer
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs user interfaces following WCAG accessibility standards and modern design patterns"
)
```

**생성될 에이전트**:
- 이름: `ui-designer`
- 모델: Sonnet
- 스킬: moai-domain-frontend, moai-accessibility-expert
- 복잡도: 높음

---

#### ✅ CSS Specialist
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that optimizes CSS, creates responsive layouts, and implements design systems with Tailwind/SCSS"
)
```

**생성될 에이전트**:
- 이름: `css-specialist`
- 모델: Haiku (실행 중심)
- 스킬: moai-lang-html-css
- 시간: <5분

---

### 3️⃣ 데이터베이스 (Database)

#### ✅ Database Schema Designer
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs database schemas with normalization, indexes, and migration strategies for PostgreSQL"
)
```

**생성될 에이전트**:
- 이름: `schema-designer`
- 모델: Sonnet
- 스킬: moai-domain-database
- 도구: Read, Write, Edit, Bash

---

#### ✅ Query Optimizer
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that optimizes SQL queries, analyzes query plans, and suggests indexing strategies"
)
```

**생성될 에이전트**:
- 이름: `query-optimizer`
- 모델: Sonnet (분석 필요)
- 스킬: moai-domain-database, moai-essentials-perf
- 시간: 15-20분

---

### 4️⃣ 보안 (Security)

#### ✅ Security Auditor
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that performs comprehensive security audits checking OWASP Top 10 vulnerabilities, encryption, and authentication patterns"
)
```

**생성될 에이전트**:
- 이름: `security-auditor`
- 모델: Sonnet (복잡한 분석)
- 스킬: moai-domain-security, moai-essentials-debug
- 시간: 20-30분

---

#### ✅ Authentication Designer
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs secure authentication systems with JWT, OAuth2, MFA, and session management"
)
```

**생성될 에이전트**:
- 이름: `auth-designer`
- 모델: Sonnet
- 스킬: moai-domain-security
- 도구: Read, Write, WebFetch, AskUserQuestion

---

#### ✅ Cryptography Expert
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that advises on encryption, key management, hashing algorithms, and cryptographic best practices"
)
```

**생성될 에이전트**:
- 이름: `crypto-expert`
- 모델: Sonnet
- 스킬: moai-domain-security
- 복잡도: 높음

---

### 5️⃣ DevOps / 배포 (DevOps)

#### ✅ Docker Specialist
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs Docker containerization strategies, Dockerfile optimization, and container security"
)
```

**생성될 에이전트**:
- 이름: `docker-specialist`
- 모델: Sonnet
- 스킬: moai-domain-devops, moai-domain-cloud
- 시간: 15-20분

---

#### ✅ Kubernetes Architect
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs Kubernetes deployments, resource management, networking, and high availability patterns"
)
```

**생성될 에이전트**:
- 이름: `kubernetes-architect`
- 모델: Sonnet (복잡한 설계)
- 스킬: moai-domain-devops, moai-domain-cloud
- 시간: 20-30분

---

#### ✅ CI/CD Pipeline Designer
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs CI/CD pipelines with GitHub Actions, GitLab CI, or Jenkins for automated testing and deployment"
)
```

**생성될 에이전트**:
- 이름: `cicd-designer`
- 모델: Sonnet
- 스킬: moai-domain-devops
- 도구: Read, Write, Edit, Bash

---

### 6️⃣ 성능 최적화 (Performance)

#### ✅ Performance Optimizer
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that profiles code, identifies bottlenecks, and recommends performance optimizations for applications"
)
```

**생성될 에이전트**:
- 이름: `performance-optimizer`
- 모델: Sonnet (분석 중심)
- 스킬: moai-essentials-perf
- 시간: 15-20분

---

#### ✅ Caching Strategist
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs caching strategies using Redis, CDN, and in-memory caches for optimal performance"
)
```

**생성될 에이전트**:
- 이름: `cache-strategist`
- 모델: Sonnet
- 스킬: moai-essentials-perf
- 복잡도: 중간

---

### 7️⃣ 테스트 (Testing)

#### ✅ Test Strategy Designer
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs comprehensive test strategies including unit, integration, E2E tests, and coverage analysis"
)
```

**생성될 에이전트**:
- 이름: `test-strategist`
- 모델: Sonnet
- 스킬: moai-domain-testing
- 시간: 15-20분

---

#### ✅ Test Code Generator
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that generates test cases using pytest, Jest, Vitest with high coverage for Python and JavaScript"
)
```

**생성될 에이전트**:
- 이름: `test-generator`
- 모델: Sonnet
- 스킬: moai-lang-python, moai-lang-typescript
- 도구: Read, Write, Edit

---

### 8️⃣ 코드 품질 (Code Quality)

#### ✅ Code Formatter
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that formats Python code using Black and enforces PEP 8 standards"
)
```

**생성될 에이전트**:
- 이름: `code-formatter`
- 모델: Haiku (빠른 실행)
- 스킬: moai-lang-python
- 시간: <5분

---

#### ✅ Linter & Style Checker
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that checks code quality with pylint, flake8, and ruff for Python projects"
)
```

**생성될 에이전트**:
- 이름: `linter-expert`
- 모델: Haiku
- 스킬: moai-lang-python
- 도구: Read, Bash, Grep

---

#### ✅ Refactoring Expert
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that analyzes code structure, identifies technical debt, and recommends refactoring strategies"
)
```

**생성될 에이전트**:
- 이름: `refactor-expert`
- 모델: Sonnet (분석 필요)
- 스킬: moai-essentials-refactor
- 시간: 15-20분

---

### 9️⃣ 문서화 (Documentation)

#### ✅ Documentation Generator
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that generates API documentation, README files, and architecture diagrams from code"
)
```

**생성될 에이전트**:
- 이름: `docs-generator`
- 모델: Sonnet
- 스킬: moai-docs-generation
- 도구: Read, Write, Edit, WebFetch

---

#### ✅ API Documentation Specialist
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that creates OpenAPI/Swagger specifications and API documentation from code"
)
```

**생성될 에이전트**:
- 이름: `api-docs-specialist`
- 모델: Sonnet
- 스킬: moai-api-designer
- 시간: 15-20분

---

### 🔟 데이터 과학 (Data Science)

#### ✅ Data Pipeline Designer
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create an agent that designs data pipelines with data validation, transformation, and quality checks"
)
```

**생성될 에이전트**:
- 이름: `pipeline-designer`
- 모델: Sonnet
- 스킬: moai-domain-data-science
- 시간: 20-30분

---

---

## 📊 에이전트 생성 통계

| 카테고리 | 에이전트 수 | 예상 시간 | 모델 |
|---------|-----------|---------|------|
| 백엔드 | 3개 | 15-30분 | Sonnet |
| 프론트엔드 | 3개 | 10-20분 | Sonnet |
| 데이터베이스 | 2개 | 15-25분 | Sonnet |
| 보안 | 3개 | 20-30분 | Sonnet |
| DevOps | 3개 | 15-30분 | Sonnet |
| 성능 최적화 | 2개 | 15-20분 | Sonnet |
| 테스트 | 2개 | 15-20분 | Sonnet |
| 코드 품질 | 3개 | 5-20분 | Haiku/Sonnet |
| 문서화 | 2개 | 15-20분 | Sonnet |
| 데이터 과학 | 1개 | 20-30분 | Sonnet |

**총계**: 26개 에이전트 생성 가능

---

## 🚀 빠른 생성 예제

### 가장 간단한 에이전트 (1단계)
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create a Python code formatter agent"
)
# 예상 시간: <5분
# 모델: Haiku
```

### 중간 난이도 에이전트 (2단계)
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create a REST API designer agent with security best practices"
)
# 예상 시간: 15-20분
# 모델: Sonnet
```

### 고난이도 에이전트 (3단계)
```bash
Task(
  subagent_type="agent-factory",
  prompt="Create a comprehensive security auditor agent that checks OWASP vulnerabilities and encryption patterns"
)
# 예상 시간: 20-30분
# 모델: Sonnet
```

---

## 💡 팁

1. **간단한 것부터**: 포매터부터 시작하여 복잡한 에이전트로 진행
2. **도메인별 그룹화**: 같은 도메인의 에이전트들은 스킬을 공유 가능
3. **팀 협업**: 각 팀원이 특정 도메인의 에이전트 생성 담당
4. **생산성**: 26개 에이전트를 수동으로 만드는 것 vs Agent Factory 사용
   - 수동: 약 100시간+ (1에이전트당 2-3시간)
   - Agent Factory: 약 15-20시간 (자동 생성)
   - **절약**: 80시간+ ⏱️

---

**어느 에이전트부터 생성해볼까요?** 💬
