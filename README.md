# Student Walkthrough Scenario: Manual Profile Loading with Simple Git Extension

**Date:** July 22, 2025 at 9:58 AM ET

**Subject:** Simplified VS Code Onboarding with Manual Profile Management and Basic Git Setup

**Purpose:** Streamlined approach using manual profile loading and a simple Git configuration extension for reliable student onboarding

---

## Scenario Overview

This walkthrough demonstrates a **simplified, reliable approach** where students manually load a pre-configured VS Code profile and use a minimal extension focused solely on Git configuration. This approach prioritizes **consistency and reliability** over full automation.

**Student Profile:**
- **Name**: Sarah Johnson
- **Course**: Web Development I
- **Assignment**: VS Code Environment Setup and Git Configuration
- **Experience Level**: Beginner (may or may not have existing VS Code setup)

**Key Changes from v5:**
- **Manual profile loading** using VS Code's built-in profile import
- **Simple Git-only extension** for basic configuration
- **Reduced complexity** with proven, reliable methods
- **Focus on core learning objectives** without automation complications

---

## Pre-Scenario Setup (Instructor Actions)

### Step 1: Extension Development
**Instructor/Department has completed:**
- Developed **Git Configurator for Grid** - Simple extension focused only on Git setup
- Extension prompts for Git username/email and sets global configuration
- Extension creates `git-config-check.txt` verification file
- No profile management - keeps extension simple and reliable

### Step 2: Course-Specific Easy-Setup Repository
**Each course has its own easy-setup repository containing:**
```
web-dev-1-easy-setup/              # Course-specific repository
├── Web Development I.code-profile  # Pre-built VS Code profile for manual import
├── git-configurator-for-grid.vsix  # Simple Git configuration extension
├── README.md                       # Step-by-step manual instructions
├── index.html                      # Course welcome page
├── welcome-cats-dots.svg           # Course assets
└── .gitignore                      # Git ignore rules
```

### Step 3: Profile Content
**The `.code-profile` file includes:**
- **Editor Settings**: 16px font, rulers at 80 columns, auto-save
- **Git Integration**: Auto-fetch, smart commits, merge editor
- **HTML/CSS Tools**: HTMLHint, Stylelint with student-friendly rules
- **Required Extensions**: Live Server, Path Intellisense, Color Highlight
- **Development Environment**: Optimized for course requirements

---

## Student Walkthrough Scenario

### Step 1: Assignment Acceptance (Student Action)
**Time**: Day 1 of assignment
**Learning Objective**: Experience GitHub Classroom workflow and learn Git clone using VS Code

**Student Action:**
1. Sarah clicks the GitHub Classroom assignment link provided in Canvas
2. GitHub Classroom creates her personal repository: `student-web-dev-1-onboarding-sarah-johnson`
3. In her web browser, she clicks the green "Code" button and copies the repository URL
4. Opens VS Code and uses the **Source Control panel** to clone:
   - Clicks the **Source Control icon** in the Activity Bar (or `Ctrl+Shift+G`)
   - Clicks **"Clone Repository"** button
   - Pastes the GitHub URL
   - Selects local folder location
   - Clicks **"Open"** when prompted

**Learning Achievement:**
- Successfully performed **Git clone** operation using VS Code interface
- Understands repository structure and workspace concept

**Student Experience:**
- Repository opens automatically in VS Code
- Sees the assignment files in VS Code Explorer
- Notices the `.code-profile` file and extension file
- Reads the README.md for step-by-step instructions

### Step 2: Manual Profile Import (Student Action)
**Time**: First 5 minutes of work session
**Learning Objective**: Learn VS Code profile management through hands-on experience

**Student Action (Following README Instructions):**
1. Sarah clicks the **profile icon** in the bottom-left corner of VS Code (gear icon or profile name)
2. From the dropdown menu, selects **"Import Profile..."**
3. Chooses **"Select File"** option
4. Navigates to and selects `Web Development I.code-profile` from her project
5. VS Code shows profile import dialog with preview of settings and extensions
6. She reviews the profile contents:
   - **Name**: Web Development I
   - **Icon**: 🎓 (graduation cap)
   - **Extensions**: HTMLHint, Live Server, Path Intellisense, Stylelint, Color Highlight
   - **Settings**: Editor preferences, Git configuration, HTML/CSS tools
7. Clicks **"Create Profile"** to import
8. Profile is created and automatically activated

**Learning Achievement:**
- Learns VS Code profile system through direct interaction
- Understands profile contents and benefits
- Gains hands-on experience with VS Code interface

**Student Experience:**
```
✓ Profile 'Web Development I' imported successfully
✓ Extensions will be installed automatically
✓ Settings applied to new profile
✓ Profile is now active
```

### Step 3: Extension Installation for Git Setup (Student Action)
**Time**: 2-3 minutes after profile import
**Learning Objective**: Install VS Code extensions and configure Git

**Student Action:**
1. Sarah follows the README instructions to install the Git configuration extension
2. Opens Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`)
3. Types: `Extensions: Install from VSIX...`
4. Selects the `git-configurator-for-grid.vsix` file from her project
5. Extension installs successfully

**Learning Achievement:**
- Learns how to install VS Code extensions from files
- Understands extension ecosystem

**Student Experience:**
```
✓ Extension 'Git Configurator for Grid' was successfully installed.
```

### Step 4: Git Configuration Setup (Student Action)
**Time**: 2-3 minutes after extension installation
**Learning Objective**: Learn Git identity configuration for version control

**Student Action:**
1. Sarah opens Command Palette (`Ctrl+Shift+P`)
2. Types: `Configure Git For Grid`
3. Extension launches Git configuration dialog

**Git Setup Dialog:**
```
📝 Git Configuration Setup

Git is essential for version control and collaboration. This configuration will be used when creating commits. The user.name and user.email are embedded in each commit's data, so they appear in your project's source control history and label who made each change.

Please enter your information:

Name: [                     ] ⚠️ Required
Email: [                     ] ⚠️ Required

This will be saved as your global Git configuration.

[ Save Git Settings ]
```

**Student Action:**
- Enters her full name: "Sarah Johnson"
- Enters her email: "sarah.johnson@student.edu"
- Clicks "Save Git Settings"

**Extension Response:**
```
✅ Git Configuration Complete!

Your Git identity has been set:
Name: Sarah Johnson
Email: sarah.johnson@student.edu

A verification file has been created: git-config-check.txt

You're ready to make commits!
```

**What Happens:**
- Extension sets global Git configuration using `git config --global`
- Creates `git-config-check.txt` file with verification details:
  ```
  Git Configuration Verification
  =============================
  
  Student: Sarah Johnson
  Email: sarah.johnson@student.edu
  Configuration Date: 2025-07-22 10:15:23 ET
  
  Git Global Configuration:
  - user.name: Sarah Johnson ✓
  - user.email: sarah.johnson@student.edu ✓
  
  Status: Ready for version control operations
  Extension: Git Configurator for Grid
  ```

**Learning Achievement:**
- Understands Git identity importance for collaboration
- Sees direct connection between identity and version control
- Experiences professional development setup

### Step 5: Environment Testing with Live Server (Student Action)
**Time**: 5-10 minutes
**Learning Objective**: Test development environment and understand Live Server workflow

**Student Action:**
1. Sarah notices that her profile includes Live Server extension (installed automatically)
2. Opens `index.html` in the editor
3. Right-clicks in the editor and selects **"Open with Live Server"**
   - **Alternative**: Clicks **"Go Live"** button in status bar
4. Live Server opens the welcome page in her default browser
5. Views the course welcome page with styling and assets
6. Makes a small edit to `index.html` (e.g., adds her name to a welcome message)
7. Saves the file and observes live reload in browser

**Learning Achievement:**
- Understands live development server concept
- Experiences real-time development workflow
- Sees immediate feedback from code changes

**Student Experience:**
- Browser opens to `http://127.0.0.1:5500/index.html`
- Welcome page displays with course branding and instructions
- Changes appear instantly in browser when files are saved
- Professional development workflow demonstrated

### Step 6: First Git Commit with Setup Verification (Student Action)
**Time**: 5-10 minutes
**Learning Objective**: Complete Git workflow with setup documentation

#### Step 6a: Observing Changes
**Student Action:**
1. Sarah notices the **Source Control icon** shows a number badge (indicating changes)
2. Clicks the **Source Control icon** (or `Ctrl+Shift+G`)
3. **Source Control panel** opens showing:
   - **Changes** section with modified files
   - **Staged Changes** section (initially empty)

**Files she sees:**
- `git-config-check.txt` (U) - Untracked file created by extension
- `index.html` (M) - Modified during Live Server testing
- Any other files she may have modified

#### Step 6b: Review Setup Documentation
**Student Action:**
- Clicks on `git-config-check.txt` to review the contents
- Understands this documents her Git configuration for the instructor
- Sees that her identity is properly configured for collaboration

#### Step 6c: Staging and Committing Changes
**Student Action:**
1. In Source Control panel, clicks the **"+"** button next to each changed file to stage them
   - Alternatively: Clicks **"+"** next to "Changes" to stage all files
2. In the commit message box, types:
   ```
   Complete VS Code environment setup and Git configuration
   
   - Imported Web Development I profile with course settings
   - Configured Git identity for version control
   - Tested Live Server development environment
   - Ready for course assignments
   ```
3. Clicks the **checkmark icon** (✓) to commit

**Learning Achievement:**
- Understands staging vs. committing
- Creates descriptive, professional commit messages
- Documents setup completion for instructor verification

### Step 7: Pushing to GitHub and Assignment Completion (Student Action)
**Time**: 2-3 minutes
**Learning Objective**: Complete full Git workflow and assignment submission

#### Step 7a: Push to Remote Repository
**Student Action:**
1. In **Source Control panel**, clicks **"Sync Changes"** button (or cloud icon)
2. VS Code pushes commit to GitHub
3. Success message appears: "Successfully pushed to origin/main"

#### Step 7b: Assignment Submission Verification
**Student Action:**
1. Opens her GitHub repository in web browser
2. Verifies that `git-config-check.txt` is present and contains her information
3. Confirms commit message appears in repository history
4. Reviews that all assignment requirements are met:
   - ✅ VS Code profile imported and active
   - ✅ Git configuration completed
   - ✅ Live Server tested successfully
   - ✅ First commit made and pushed
   - ✅ Setup verification file created

**Learning Achievement:**
- Completes full Git workflow from local changes to remote repository
- Understands importance of setup verification
- Gains confidence in development environment

---

## Instructor Experience with Simplified Approach

### Grading Benefits

#### Easy Verification
**Instructor can quickly check:**
1. **git-config-check.txt** confirms proper Git configuration
2. **Commit history** shows professional commit messages
3. **Repository activity** demonstrates successful environment setup
4. **Profile usage** evident from standardized development workflow

#### Reduced Support Burden
**Simplified approach eliminates:**
- Complex extension automation issues
- Profile creation failures
- Name conflict problems
- Automation timing issues

### Success Indicators
**Clear evidence of success:**
- Git configuration file present with student information
- Commit made with proper Git identity
- Professional commit message structure
- Repository successfully updated on GitHub

---

## Advantages of Manual Profile Approach

### Reliability Benefits
1. **Uses VS Code's native profile system** - No custom automation
2. **Student learns profile management** - Valuable skill for career
3. **Eliminates automation failures** - Consistent success rate
4. **Simpler troubleshooting** - Fewer moving parts

### Educational Benefits
1. **Hands-on learning** - Students interact directly with VS Code features
2. **Profile understanding** - Clear connection between actions and results
3. **Professional workflow** - Industry-standard profile management
4. **Transferable skills** - Applicable beyond course context

### Technical Benefits
1. **No API dependencies** - Uses stable VS Code functionality
2. **Cross-platform compatibility** - Works identically on all systems
3. **Version independence** - Not affected by VS Code API changes
4. **Predictable behavior** - Manual steps have consistent outcomes

---

## Extension Simplification Benefits

### Git Configurator for Grid Features
**Simple, focused functionality:**
- Prompts for Git username and email
- Sets global Git configuration
- Creates verification file
- No profile management complexity

### Reduced Risk
**Eliminates potential issues:**
- Profile creation failures
- Extension installation conflicts
- Settings application problems
- Complex automation timing

### Easier Maintenance
**Simplified codebase:**
- Single-purpose extension
- Minimal dependencies
- Easy to test and debug
- Straightforward updates

---

## Student Learning Outcomes

### Technical Skills Gained
1. **VS Code Profile Management**: Manual import and activation
2. **Extension Installation**: From .vsix files
3. **Git Configuration**: Understanding identity setup for collaboration
4. **Live Server Usage**: Real-time development environment
5. **Version Control Workflow**: Complete Git commit and push cycle

### Professional Development
1. **Environment Setup**: Hands-on configuration experience
2. **Tool Proficiency**: Direct interaction with development tools
3. **Documentation Skills**: Creating verification files and commit messages
4. **Problem-Solving**: Manual approach builds understanding
5. **Industry Practices**: Profile management and Git workflows

---

## Assignment Completion Checklist

### For Students
- [ ] Repository cloned to local machine
- [ ] VS Code profile imported from `.code-profile` file
- [ ] Profile "Web Development I" is active (visible in bottom-left corner)
- [ ] Git Configurator extension installed from `.vsix` file
- [ ] Git identity configured (name and email)
- [ ] `git-config-check.txt` file created by extension
- [ ] Live Server tested with `index.html`
- [ ] Changes committed with descriptive message
- [ ] Commit pushed to GitHub repository

### For Instructors
- [ ] `git-config-check.txt` present in student repository
- [ ] Git configuration contains valid student information
- [ ] Commit history shows proper identity in commit author
- [ ] Commit message demonstrates understanding of setup process
- [ ] Repository updated successfully on GitHub

---

## Troubleshooting Guide

### Common Issues and Solutions

#### Profile Import Fails
**Issue**: Cannot import `.code-profile` file
**Solution**: 
1. Ensure VS Code is updated to recent version
2. Check file is not corrupted (try opening in text editor)
3. Use Command Palette: "Preferences: Import Profile..."
4. Contact instructor if file appears damaged

#### Extension Won't Install
**Issue**: Cannot install `.vsix` file
**Solution**:
1. Use Command Palette: "Extensions: Install from VSIX..."
2. Ensure file downloaded completely
3. Try restarting VS Code
4. Check VS Code version compatibility

#### Git Configuration Doesn't Work
**Issue**: Extension doesn't prompt for Git information
**Solution**:
1. Open Command Palette and search "Configure Git For Grid"
2. Ensure extension is activated (check Extensions panel)
3. Try reloading VS Code window
4. Manually run git config commands if needed

#### Live Server Not Working
**Issue**: Live Server extension not available
**Solution**:
1. Check that profile was imported correctly
2. Manually install Live Server from Extensions marketplace
3. Ensure no conflicting extensions are installed
4. Try right-clicking HTML file and selecting "Open with Live Server"

---

## Success Metrics

### Quantitative Goals
- **100%** profile import success rate (using VS Code native functionality)
- **< 5 minutes** total setup time
- **98%** successful Git configuration
- **Zero** automation-related failures
- **100%** assignment completion rate

### Qualitative Benefits
- **Enhanced student understanding** through hands-on interaction
- **Reduced instructor support burden** due to simpler approach
- **Increased student confidence** with predictable outcomes
- **Better learning retention** through manual skill development
- **Professional skill building** with industry-standard tools

---

## Conclusion

The **Manual Profile Loading with Simple Git Extension** approach represents a **reliable, educational solution** that prioritizes student learning and success over automation complexity. By using VS Code's native features and focusing on core learning objectives, we achieve:

### Core Benefits
1. **Maximum Reliability**: Uses proven VS Code functionality
2. **Enhanced Learning**: Students gain hands-on experience with tools
3. **Professional Skills**: Industry-standard profile and Git management
4. **Simplified Support**: Fewer points of failure
5. **Consistent Success**: Predictable outcomes across all students

### Student Empowerment
- **Direct Tool Interaction**: Understanding through hands-on experience
- **Professional Skills**: Profile management applicable to career
- **Confidence Building**: Success through reliable, tested methods
- **Problem-Solving**: Understanding tools enables independent troubleshooting

### Institutional Excellence
- **Reliable Outcomes**: Consistent success across all students
- **Reduced Support**: Simpler approach requires less troubleshooting
- **Professional Preparation**: Students learn industry-standard practices
- **Scalable Solution**: Manual approach works for unlimited students
- **Cost Effective**: Minimal development and maintenance overhead

This manual approach positions students for success while teaching valuable professional skills that will serve them throughout their careers in software development.
