# Confrmd Development Guidelines

## Code Quality Standards

**ZERO WARNINGS POLICY**: All code must compile without warnings. Any compiler warnings, package warnings, or code analysis warnings must be fixed immediately. We maintain a warning-free codebase.

### Warning Resolution Guidelines
- **NU1510 (Package warnings)**: Remove unnecessary package references
- **CS8618 (Nullable warnings)**: Add `required` modifier or initialize properties
- **CS0414 (Unused fields)**: Remove unused code or suppress with justification
- **Build warnings**: Fix immediately before committing

## Documentation Maintenance

**CRITICAL**: When making changes that affect how the application works, its architecture, flow, or implementation, ALWAYS update the documentation to reflect those changes. Documentation must be kept in sync with the codebase.

### When to Update Documentation

Update documentation files whenever you:
1. **Change Architecture or Design** - Update system design or module structure
2. **Add/Modify Features** - Document new functionality or changes to existing features
3. **Change Configuration** - Update environment variables or configuration documentation
4. **Modify API Endpoints** - Document new/changed endpoints, request/response formats
5. **Update Dependencies** - Document framework version changes
6. **Change Build/Deploy Process** - Update build commands, deployment steps
7. **Add Styling** - Document new CSS classes, components, or design patterns

### Files to Update

When making changes, review and update these documentation files as appropriate:

**Core Documentation:**
- `README.md` - Main repository README (features, quick start, tech stack)
- `docs/architecture.md` - System architecture (create if needed)
- `docs/development.md` - Development setup, local running (create if needed)
- `docs/deployment.md` - Deployment procedures, environment configuration (create if needed)
- `docs/api.md` - API reference and endpoint documentation (create if needed)

### Documentation Standards

**Be Specific and Accurate:**
- ✅ Use actual file paths, not placeholders
- ✅ Include real code examples from the codebase
- ✅ Reference specific version numbers
- ✅ Update badges and status indicators
- ✅ Keep command examples up to date

**Maintain Consistency:**
- ✅ Use the same terminology across all docs
- ✅ Keep directory structure references accurate
- ✅ Update all related documentation together
- ✅ Cross-reference related docs with links

**Include Context:**
- ✅ Explain WHY changes were made, not just WHAT changed
- ✅ Document tradeoffs and design decisions
- ✅ Include troubleshooting sections for common issues
- ✅ Add validation/testing steps

### Documentation Update Workflow

1. **During Development:**
   - Note which documentation files need updates as you code
   - Keep a list of changes that affect public APIs or architecture

2. **Before Committing:**
   - Review the list of documentation files that need updates
   - Update all relevant documentation in the same commit as code changes
   - Verify all links, code examples, and file paths are correct

3. **In Pull Request:**
   - List documentation updates in the PR description
   - Ensure reviewers check both code AND documentation changes
   - Documentation quality is as important as code quality

### Documentation is Not Optional

Treating documentation as a first-class deliverable ensures:
- New developers can onboard quickly
- Features are discoverable and understandable
- Architecture decisions are preserved
- The codebase remains maintainable over time

**Remember:** If the code changed, the documentation should change too!

---

## Git Workflow
As part of any changes you make, put a git commit in describing what was done.

```
git add .
git commit -m "Describe the changes made"
git push origin your-branch-name
```

## Project Structure

### Confrmd Project
- **Location**: Root directory
- **Type**: Configuration/Tools Repository
- **Purpose**: Supporting project for ecosystem tools

### Build Requirements
**CRITICAL**: When making changes, ALWAYS:
1. **Update documentation** reflecting any changes
2. **Test thoroughly** before committing
3. **Verify any configuration** is accurate
4. **Create descriptive git commits**
5. **Align** with ecosystem guidelines

## Code Standards

### Naming Conventions
- **Files**: Use meaningful, descriptive names
- **Directories**: Organize logically by feature or function
- **Configuration**: Use clear, searchable variable names

### Error Handling
- Log all errors with context
- Provide meaningful error messages
- Document expected errors and recovery steps

### Testing
- Document testing procedures
- Include validation steps in README
- Provide examples for verification

## Development Notes

### Best Practices
- Keep documentation updated
- Follow ecosystem guidelines
- Test thoroughly before committing
- Use clear, descriptive commit messages
- Reference related issues or PRs

### Common Tasks
- Review README.md for project purpose
- Update README.md with new features
- Document configuration changes
- Commit changes with descriptive messages

## Alignment with Ecosystem

This project follows the same guidelines as all Rejist ecosystem projects:
- Zero warnings policy
- Documentation-first approach
- Standardized git workflow
- Consistent code standards
- Aligned architecture patterns

---

**Last Updated**: January 21, 2026  
**Version**: 1.0  
**Aligned with**: Rejist Development Guidelines
