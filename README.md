# FN7 Micro Module Template

This is a template repository that can be used as a starting point for building FN7 micro modules. Micro modules are standalone applications that integrate with the FN7 platform using the provided SDKs.

## 🚀 Quick Start

### Option 1: Use GitHub Template Feature (Recommended)

1. Click the green **"Use this template"** button on GitHub
2. Give your new repository a name
3. Click **"Create repository from template"**
4. Clone your new repository
5. You're done! The new repository is already disconnected from this template.

### Option 2: Manual Setup

1. **Clone the repository:**
   ```bash
   git clone <this-repo-url>
   cd <repo-name>
   ```

2. **Remove the existing git history:**
   ```bash
   rm -rf .git
   git init
   git add .
   git commit -m "Initial commit from template"
   ```

3. **Create a new repository** on GitHub/GitLab/Bitbucket (do NOT initialize with README)

4. **Add your remote and push:**
   ```bash
   git remote add origin <your-new-repo-url>
   git branch -M main
   git push -u origin main
   ```

## 📦 Building a Micro Module

FN7 micro modules can be built using either frontend or backend SDKs, depending on your use case.

### Frontend Micro Modules

For building frontend applications (React, Angular, Vue, or vanilla JavaScript), use the **FN7 Frontend SDK**.

**Key Features:**
- Firebase CRUD operations (Get, Create, Update, Delete, Search)
- Firebase Storage operations (Upload, Get URL, Get Blob)
- User, Application, and Organization context helpers
- Real-time Firebase listeners
- Framework-agnostic (works with React, Angular, Vue, etc.)

**Documentation:** See [`fn7-sdk/frontend-sdk.md`](./fn7-sdk/frontend-sdk.md) for complete API reference and usage examples.

**Example Implementation:** Check out [fn7SDK-React-app](https://github.com/d1nzfn7/fn7SDK-React-app) for a working React implementation.

**Installation:**
```html
<!-- CDN -->
<script src="https://fn7.io/.fn7-sdk/frontend/latest/sdk.min.js"></script>

<!-- Or ES Modules -->
<script type="module">
  import { SDK } from 'https://fn7.io/.fn7-sdk/frontend/latest/sdk.esm.js';
</script>
```

### Backend Micro Modules

For building backend APIs and services (Python), use the **FN7 Python SDK**.

**Key Features:**
- Firebase CRUD operations with security rules enforcement
- Firebase Storage operations
- JWT token-based authentication
- Organization isolation and access control
- Built-in security validation

**Documentation:** See [`fn7-sdk/python-sdk.md`](./fn7-sdk/python-sdk.md) for complete API reference and usage examples.

**Example Implementation:** Check out [fn7SDK-python-backend](https://github.com/d1nzfn7/fn7SDK-python-backend) for a working FastAPI backend implementation.

**Installation:**
```bash
pip install fn7-sdk --index-url https://fn7.io/.fn7-sdk/python/
```

## 📚 SDK Documentation

Both SDKs are documented in detail:

- **Frontend SDK:** [`fn7-sdk/frontend-sdk.md`](./fn7-sdk/frontend-sdk.md) - Complete API reference for JavaScript/TypeScript SDK
- **Python SDK:** [`fn7-sdk/python-sdk.md`](./fn7-sdk/python-sdk.md) - Complete API reference for Python SDK

## 🎨 UI Guidelines

For frontend micro modules, please refer to [`UI_CONTEXT.md`](./UI_CONTEXT.md) for design guidelines, including:
- Font specifications (Sora)
- Theme requirements (Light theme)
- Color palette
- Component guidelines

## 📝 Next Steps

After setting up your repository:

1. Choose your stack (Frontend or Backend)
2. Review the appropriate SDK documentation
3. Check out the example implementations for reference
4. Start building your micro module!

## ⚠️ Important Notes

- **Never push directly to this template repository** - Always create a new repository first
- Both SDKs require proper Firebase configuration and authentication
- Review the example implementations for best practices
- Follow the UI guidelines for frontend modules

## 🤝 Contributing to the Template

If you want to improve this template itself, please:

1. Fork this repository
2. Make your changes
3. Submit a pull request

---

**Note:** If you're using this template on GitHub, make sure the repository settings mark it as a template repository (Settings → Template repository).
