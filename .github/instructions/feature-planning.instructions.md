---
description: 'Guidelines for creating high-quality custom instruction files for GitHub Copilot'
applyTo: '**'
---

# Planning New Features

When designing new features, you should:

- Create a plan file with a `.tmp` extension at the root of the project
- Ensure that `.tmp` files are ignored by version control
- Review all existing documentation and code related to the area of the codebase where the new feature will be implemented to understand the current state and any relevant constraints or considerations
- Document the feature design in the plan file using a structured format with the following sections: Feature Description, Requirements (including user stories and acceptance criteria), Documentation and Tests, and Implementation Plan
- Include a dedicated section for documentation and test changes, identifying updates to existing documentation or tests as well as any new documentation or tests that will need to be created
- Consider the impact of the new feature on existing code and functionality, and plan for any necessary refactoring or adjustments
- Interview me to gather requirements and clarify any uncertainties about the feature, asking one question at a time and integrating responses into the plan document
- Identify risks in the feature and propose mitigation strategies to address those risks in the implementation plan, interviewing me to make decisions about how to address the risks
- Create an implementation plan that outlines the steps needed to build the feature, including any necessary changes to existing code or infrastructure
- Break the plan into logical phases or milestones, and set clear goals for each phase, including phase exit criteria that define when the phase is complete and ready to move on to the next phase
- Do not begin implementing the feature until the plan has been reviewed and approved; notify me when the plan is ready for review
- Regularly review and update the plan as needed based on feedback and new information
- Refer back to the plan regularly during implementation to ensure you are following the steps outlined and meeting the requirements identified
- Check in regularly during implementation to provide progress updates and get feedback, and notify me of any significant changes to the plan
- Ensure that the implementation plan is realistic and achievable, and adjust it as necessary based on any challenges or obstacles that arise during development
- Include appropriate testing and validation steps in the implementation plan to ensure that the feature is working as intended and does not introduce any regressions or issues into the codebase
