# pkgbuild-template-translator

Template for creating Arch Linux packages with automatic translation support for Community Big Linux.

## 🚀 Features

- Basic structure for Arch Linux packages
- Integrated automatic translation using OpenAI
- Integration with Community Big build system
- Configured GitHub Actions workflow
- TMATE support for debugging

## 📋 Prerequisites

To use this template, you need:

1. A GitHub account
2. Configure the following secrets in your repository:
   - `OPENAI_KEY`: OpenAI API key for translations
   - `TOKEN_RELEASE`: Token for build system integration
   - Other tokens will be inherited automatically

## 🛠️ Repository Structure

```
.
├── .github/
│   └── workflows/
│       └── translate-and-build-package.yml
├── PKGBUILD
├── pkgbuild.install
├── README.md
└── LICENSE
```

## 📦 How to Use

1. Click "Use this template" on GitHub
2. Configure the required secrets in Settings > Secrets and variables > Actions
3. Modify the PKGBUILD as needed
4. Push your changes

The workflow will run automatically:
- On every push
- Manually through the GitHub Actions interface

## 🔄 Translation Workflow

The translation process runs automatically and includes:
1. Installing required dependencies
2. Cloning big-auto-translator
3. Executing translation
4. Committing and pushing changes
5. Triggering package build

## 🐛 Debugging

To debug the workflow:
1. Go to Actions > Translate and Build Package
2. Click "Run workflow"
3. Check "With TMATE" for interactive debugging session

## 📄 License

This project is under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Contributing

Contributions are welcome! Please feel free to submit pull requests or create issues.

## 🌐 Translation Support

This template automatically handles translations for:
- Package descriptions
- Installation messages
- Documentation
- User interface elements

The translation system uses OpenAI's API to ensure high-quality translations while maintaining technical accuracy.
