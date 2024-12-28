# APIOps Cycles Prompt Framework

## Overview
This framework defines how prompts should be structured and chained together through the APIOps Cycles method phases. It ensures context preservation and consistent outputs across the entire API lifecycle.

## Global Context Structure
```json
{
  "project_context": {
    "api_name": "string",
    "business_domain": "string",
    "stakeholders": [{
      "name": "string",
      "role": "string",
      "key_concerns": ["string"]
    }]
  },
  "current_phase": {
    "name": "string",
    "status": "string",
    "artifacts_produced": ["string"]
  },
  "decisions_log": [{
    "phase": "string",
    "decision": "string",
    "rationale": "string",
    "impact": "string",
    "date": "string"
  }]
}
```

## Phase 1: API Product Strategy

### Required Input Context
- Business objectives
- Target API consumers
- Current pain points
- Competitor analysis
- Resource constraints

### Expected Outputs
```json
{
  "customer_journey_map": {
    "touchpoints": ["string"],
    "pain_points": ["string"],
    "opportunities": ["string"]
  },
  "value_proposition": {
    "target_consumers": ["string"],
    "key_benefits": ["string"],
    "differentiators": ["string"]
  },
  "business_model": {
    "revenue_streams": ["string"],
    "cost_structure": ["string"],
    "key_partners": ["string"]
  }
}
```

### Transition Criteria
- Complete customer journey map
- Validated value proposition
- Approved business model
- Stakeholder sign-off

## Phase 2: API Consumer Experience

### Required Input Context
- Value proposition from Phase 1
- Target consumer segments
- Technical requirements
- Integration constraints

### Expected Outputs
```json
{
  "consumer_needs": {
    "functional": ["string"],
    "non_functional": ["string"],
    "constraints": ["string"]
  },
  "technical_requirements": {
    "data_formats": ["string"],
    "performance_criteria": ["string"],
    "security_requirements": ["string"]
  }
}
```

### Transition Criteria
- Validated consumer needs
- Documented technical requirements
- Consumer feedback incorporated

## Phase 3: API Platform Architecture

### Required Input Context
- Technical requirements from Phase 2
- Infrastructure constraints
- Security requirements
- Compliance needs

### Expected Outputs
```json
{
  "platform_architecture": {
    "components": ["string"],
    "data_flows": ["string"],
    "integration_points": ["string"]
  },
  "capacity_plan": {
    "baseline_metrics": {},
    "scaling_rules": {},
    "resource_requirements": {}
  }
}
```

### Transition Criteria
- Approved architecture design
- Validated capacity plan
- Risk assessment complete

## Phase 4: API Design

### Required Input Context
- Platform architecture from Phase 3
- Data requirements
- Interface patterns
- Design standards

### Expected Outputs
```json
{
  "api_contract": {
    "endpoints": ["string"],
    "data_models": ["string"],
    "security_schemes": ["string"]
  },
  "documentation": {
    "reference": "string",
    "examples": ["string"],
    "guides": ["string"]
  }
}
```

### Transition Criteria
- Complete API contract
- Validated against standards
- Technical review complete

## Phase 5: API Audit

### Required Input Context
- API contract from Phase 4
- Compliance requirements
- Security standards
- Performance criteria

### Expected Outputs
```json
{
  "audit_results": {
    "findings": ["string"],
    "severity_levels": ["string"],
    "recommendations": ["string"]
  },
  "remediation_plan": {
    "tasks": ["string"],
    "priorities": ["string"],
    "timeline": "string"
  }
}
```

### Transition Criteria
- All critical findings addressed
- Compliance requirements met
- Security validation complete

## Phase 6: API Publishing

### Required Input Context
- Audit results from Phase 5
- Publishing platform details
- Documentation requirements
- Support procedures

### Expected Outputs
```json
{
  "publishing_package": {
    "api_artifacts": ["string"],
    "documentation": ["string"],
    "support_materials": ["string"]
  },
  "deployment_plan": {
    "stages": ["string"],
    "rollback_procedures": ["string"],
    "monitoring_setup": ["string"]
  }
}
```

### Transition Criteria
- Documentation complete
- Deployment plan approved
- Support processes in place

## Phase 7: API Adoption

### Required Input Context
- Publishing package from Phase 6
- Adoption targets
- Success metrics
- Support resources

### Expected Outputs
```json
{
  "adoption_metrics": {
    "usage_stats": {},
    "consumer_feedback": ["string"],
    "success_indicators": ["string"]
  },
  "improvement_plan": {
    "backlog": ["string"],
    "priorities": ["string"],
    "timeline": "string"
  }
}
```

### Transition Criteria
- Adoption targets met
- Feedback loop established
- Continuous improvement plan in place

## Error Handling
Each phase should include error handling for:
- Missing required context
- Invalid inputs
- Failed validations
- Incomplete deliverables

## Context Preservation
- Each phase must preserve decisions and artifacts
- Updates to shared context must be atomic
- State changes must be tracked in decisions log

## Phase Transitions
- Explicit handoff between phases
- Validation of transition criteria
- Context verification before proceeding
