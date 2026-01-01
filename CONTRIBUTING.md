# Contributing to SEPilot Documentation

SEPilot 문서에 기여해 주셔서 감사합니다!

Thank you for contributing to SEPilot documentation!

## How to Contribute

### 1. Documentation Standards

모든 문서는 다음 표준을 따라야 합니다:

All documentation should follow these standards:

- Use Markdown (.md) format
- Use UTF-8 encoding
- Include both Korean and English content when possible
- Follow the document template (see `/templates/` directory)
- Use clear, concise language
- Include code examples where applicable

### 2. File Naming Conventions

파일명 규칙:

File naming conventions:

- Use lowercase letters
- Use hyphens (-) to separate words
- Use descriptive names
- Example: `installation-guide.md`, `api-authentication.md`

### 3. Document Structure

각 문서는 다음 구조를 포함해야 합니다:

Each document should include the following structure:

```markdown
---
title: Document Title
date: YYYY-MM-DD
category: category-name
tags: [tag1, tag2, tag3]
---

# Document Title

Brief introduction or overview

## Section 1

Content...

## Section 2

Content...
```

### 4. Metadata

문서 상단에 메타데이터를 포함하세요:

Include metadata at the top of each document:

- **title**: Document title
- **date**: Creation or last update date (YYYY-MM-DD format)
- **category**: Category (getting-started, development, api, architecture, tutorials, reference)
- **tags**: Relevant tags for searchability

### 5. Code Examples

코드 예제 작성 시:

When writing code examples:

- Use proper syntax highlighting
- Include comments for clarity
- Provide complete, runnable examples when possible
- Explain what the code does

Example:
````markdown
```python
# Example: Hello World
def greet(name):
    """Greet a user by name."""
    return f"Hello, {name}!"

# Usage
print(greet("SEPilot"))
```
````

### 6. Images and Diagrams

이미지 사용 시:

When using images:

- Store images in a `/docs/images/` directory
- Use descriptive file names
- Include alt text for accessibility
- Optimize image size

### 7. Links

링크 작성 시:

When creating links:

- Use relative links for internal documentation
- Use descriptive link text
- Verify all links work before submitting

### 8. Review Process

문서 제출 프로세스:

Document submission process:

1. Create a new branch for your changes
2. Add or modify documentation
3. Update the relevant category README to include your document
4. Submit a pull request
5. Address any review comments
6. Once approved, your contribution will be merged

## Documentation Categories

문서를 적절한 카테고리에 배치하세요:

Place your document in the appropriate category:

- **getting-started/**: Introductory content for new users
- **development/**: Development processes and best practices
- **api/**: API documentation
- **architecture/**: System architecture and design
- **tutorials/**: Step-by-step guides
- **reference/**: Technical reference materials

## Questions?

질문이 있으시면 이슈를 열어주세요.

If you have questions, please open an issue.

## License

By contributing, you agree that your contributions will be licensed under the same license as the project.
