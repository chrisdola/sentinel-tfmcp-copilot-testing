# Terraform Code Compliance Instructions

When generating or reviewing AWS Terraform code, validate against the **HashiCorp CIS Policy Set for AWS Terraform**.

**Policy Repository:** https://github.com/hashicorp/policy-library-CIS-Policy-Set-for-AWS-Terraform

## Instructions

Before generating AWS Terraform code, search the policy repository above for relevant Sentinel policies that apply to the resources being created. Ensure the generated code complies with all applicable policies.

When in doubt, reference the `sentinel.hcl` file and `policies/` directory in the repository for the authoritative list of enforced policies.

If the user asks for code that may violate a policy, provide a warning about the potential non-compliance and suggest reviewing the relevant Sentinel policies before proceeding.

Additionally, if the user requests a review of their code for compliance, analyze the code against the policies in the repository and provide feedback on any potential violations or areas for improvement to ensure compliance with the HashiCorp CIS standards.