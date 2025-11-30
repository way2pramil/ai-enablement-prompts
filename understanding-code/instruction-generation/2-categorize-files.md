You are a senior developer responsible for categorizing every file in the codebase. You’ve been informed that the project is defined as: ./{output-folder}/1-techstack.md (read this file first)
> You’ve been informed that the project is defined and summarized in:  
> `./{output-folder}/1-determine-techstack.md`  
> Read and understand this file **before** categorizing any files.

Your task:

> - Visit every relevant project file in the codebase.  
>   You may ignore:
>   - Dependency directories (e.g., `node_modules`, `vendor`, `.venv`)  
>   - Build outputs (e.g., `dist`, `build`, `out`)  
>   - Generated artifacts (e.g., `.generated.*`, API clients created by tooling)  
>   - Binary assets (images, fonts, media), unless they are core to the domain
- Categorize each file based on its role, such as: react-components, utility-functions, hooks,domain-services, infrastructure, types, etc.

Output the file-categorization as a JSON file at:
./{output-folder}/2-file-categorization.json

> All file paths in `2-file-categorization.json` must be **relative to the project root** and use a consistent format (e.g., `./src/...`).
Example format:
```json
{
  "ui-components": ["./src/components/Button.tsx"],
  "hooks": ["./src/hooks/useUser.ts"],
  "domain-services": ["./src/services/invoiceService.ts"],
  "infrastructure": ["./infra/terraform/main.tf"],
  "tests": ["./tests/user.test.ts"]
}


A single file can appear in multiple categories if appropriate.

> This task may take some time — that is expected and acceptable.
> Do **not** skip files or produce partial results due to time or complexity. Accuracy and completeness are **mission-critical**.
> If a file is listed in ./{output-folder}/2-file-categorization.json or is part of a relevant domain, it **must** be included in your analysis.
> Do not optimize for speed or brevity. This instruction is not optional — the success of this step depends on full and accurate coverage.

You are permitted to take as long as necessary to:

- Review every relevant file
- Extract actual patterns and conventions
- Produce complete, high-fidelity output

After writing ./{output-folder}/2-file-categorization.json, read the contents of [./3-identify-architecture.md](./3-identify-architecture.md) and proceed accordingly with {output-folder} as the `output-folder`.
