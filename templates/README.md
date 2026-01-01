# Documentation Templates

문서 작성을 위한 템플릿 모음입니다.

This directory contains templates for creating documentation.

## Available Templates

사용 가능한 템플릿:

Available templates:

### 1. Document Template
**File**: `document-template.md`

일반적인 문서 작성을 위한 기본 템플릿입니다.

General-purpose template for creating standard documentation.

**Use for**:
- General documentation
- How-to guides
- Concept explanations
- Process documentation

### 2. API Template
**File**: `api-template.md`

API 문서 작성을 위한 템플릿입니다.

Template for creating API documentation.

**Use for**:
- REST API endpoints
- API reference documentation
- Request/response specifications
- Authentication documentation

### 3. Tutorial Template
**File**: `tutorial-template.md`

단계별 튜토리얼 작성을 위한 템플릿입니다.

Template for creating step-by-step tutorials.

**Use for**:
- Step-by-step guides
- Hands-on tutorials
- Learning paths
- Workshop materials

## How to Use

### 1. Choose a Template

문서 유형에 맞는 템플릿을 선택하세요.

Choose the template that matches your document type.

### 2. Copy the Template

템플릿을 적절한 카테고리 디렉토리로 복사하세요.

Copy the template to the appropriate category directory.

```bash
# Example: Creating a new tutorial
cp templates/tutorial-template.md docs/tutorials/my-new-tutorial.md
```

### 3. Fill in the Content

메타데이터와 내용을 채워 넣으세요.

Fill in the metadata and content.

### 4. Update Category README

카테고리 README에 새 문서를 추가하세요.

Add your new document to the category README.

## Template Guidelines

### Metadata

모든 템플릿은 상단에 메타데이터 섹션을 포함합니다:

All templates include a metadata section at the top:

```yaml
---
title: Document Title
date: YYYY-MM-DD
category: category-name
tags: [tag1, tag2, tag3]
---
```

**Required fields**:
- `title`: Document title
- `date`: Creation date (YYYY-MM-DD)
- `category`: One of: getting-started, development, api, architecture, tutorials, reference
- `tags`: Array of relevant tags

### Structure

각 템플릿은 일관된 구조를 따릅니다:

Each template follows a consistent structure:

1. **Title and Introduction**: Clear title and overview
2. **Prerequisites**: What's needed before starting
3. **Main Content**: Detailed information organized in sections
4. **Examples**: Practical examples
5. **Additional Information**: Related docs, references, etc.

### Bilingual Content

가능한 경우 한국어와 영어를 모두 포함하세요:

When possible, include both Korean and English:

```markdown
## Section Title

Korean explanation.

English explanation.
```

## Customization

필요에 따라 템플릿을 수정할 수 있습니다:

You can customize templates as needed:

- Add or remove sections
- Adjust structure for your content
- Include additional metadata fields

템플릿은 가이드라인입니다. 문서를 더 명확하게 만드는 데 도움이 된다면 자유롭게 수정하세요.

Templates are guidelines. Feel free to adapt them if it makes your documentation clearer.

## Questions?

템플릿에 대한 질문이나 제안이 있으시면 이슈를 열어주세요.

If you have questions or suggestions about the templates, please open an issue.
