# Scenario Management Guide for Facilitators
## Critical Thinking Training Registration System

---

## 📋 Table of Contents
1. [Understanding Scenarios](#understanding-scenarios)
2. [How to Update Scenarios](#how-to-update-scenarios)
3. [Scenario Best Practices](#scenario-best-practices)
4. [Quick Update Methods](#quick-update-methods)
5. [Troubleshooting](#troubleshooting)

---

## 🎯 Understanding Scenarios

### What Are Scenarios?

Scenarios are the **critical thinking tasks** assigned to each group during your training session. Each of the four groups receives a different scenario to work on together.

### Default Scenarios

The system comes with four pre-configured scenarios:

**Group 1: The Think Tank**
```
Analyze a complex business problem: A local company is losing customers 
despite having the best prices. What non-price factors could be causing 
this, and what solutions would you recommend?
```

**Group 2: The Insight Collective**
```
Ethical dilemma: Your team developed an AI tool that could automate 60% 
of jobs in your industry. Should you release it? Discuss the trade-offs 
between innovation and social responsibility.
```

**Group 3: The Solution Studio**
```
Creative problem solving: Design a public transportation system for a 
city with extreme traffic congestion, limited budget, and resistance to 
change. What innovative solutions can you propose?
```

**Group 4: The Pathfinders**
```
Critical analysis: You've been given three conflicting research reports 
about climate change solutions. How would you evaluate their credibility 
and determine the best course of action?
```

### How Scenarios Work

1. **Participant registers** → Gets assigned to a group (round-robin)
2. **System shows confirmation** → Displays group name AND scenario
3. **Participant sees task** → "During the session, you will work with others in your group on this critical thinking task"
4. **Admin sees everything** → Dashboard shows all groups with their scenarios and participants

---

## 🔧 How to Update Scenarios

### Method 1: Admin Dashboard (Recommended)

**For Non-Technical Facilitators - No Coding Required!**

#### Option A: Edit Individual Scenarios

1. **Open Admin Dashboard**
   - URL: `https://your-project.web.app/admin.html`

2. **Locate the Group Card**
   - You'll see four colored cards, one for each group
   - Each card shows: Group name, current scenario, and participants

3. **Click "✏️ Edit" Button**
   - Located in the top-right corner of each group card
   - A popup window will appear

4. **Update the Scenario**
   - Edit the text in the text box
   - Write your new critical thinking task
   - Can be any length (recommended: 1-3 sentences)

5. **Save Changes**
   - Click "💾 Save Scenario"
   - Changes take effect immediately
   - New registrations will see the updated scenario

**Example Update:**
```
Before: "Analyze a complex business problem..."

After: "Case Study: A hospital is experiencing high staff turnover. 
Identify root causes and propose retention strategies."
```

---

#### Option B: Manage All Scenarios at Once

**Best for preparing for a new training session**

1. **Open Admin Dashboard**

2. **Click "📝 Manage All Scenarios"**
   - Green button in the action button row

3. **Edit All Four Scenarios**
   - You'll see a form with text boxes for all four groups
   - Update any or all scenarios at once
   - Review side-by-side before saving

4. **Save All Changes**
   - Click "💾 Save All Scenarios"
   - All changes applied simultaneously

**When to Use This:**
- Preparing for a new training topic
- Changing all scenarios at once
- Creating themed scenarios (e.g., all healthcare scenarios)

---

### Method 2: Direct Firebase Update (Advanced)

**For Technical Users or Bulk Updates**

1. **Open Firebase Console**
   - Go to: https://console.firebase.google.com/
   - Select your project

2. **Navigate to Realtime Database**
   - Click "Realtime Database" in the left menu
   - Click on the "Data" tab

3. **Find "scenarios" Node**
   - You'll see: `scenarios/`
   - Expand to see: `group1`, `group2`, `group3`, `group4`

4. **Edit Any Scenario**
   - Click on the scenario text
   - Edit directly in Firebase
   - Press Enter to save

5. **Or Add New Scenarios**
   - If `scenarios/` doesn't exist, create it
   - Add child nodes: `group1`, `group2`, `group3`, `group4`
   - Set values to your scenario text

**Firebase Structure:**
```
scenarios/
  ├── group1: "Your scenario for Group 1"
  ├── group2: "Your scenario for Group 2"
  ├── group3: "Your scenario for Group 3"
  └── group4: "Your scenario for Group 4"
```

---

## ✍️ Scenario Best Practices

### Writing Effective Critical Thinking Scenarios

**1. Clear and Specific**
✅ Good: "A company's new product failed despite positive market research. Analyze why this might happen and suggest prevention strategies."

❌ Too Vague: "Think about business problems."

---

**2. Appropriate Length**
- **Ideal:** 2-4 sentences
- **Maximum:** 6-8 sentences
- Participants see this on mobile devices - keep it readable

---

**3. Action-Oriented**
Use verbs that prompt thinking:
- Analyze, Evaluate, Propose, Design, Compare
- Identify, Recommend, Prioritize, Justify
- Challenge, Synthesize, Critique, Develop

---

**4. Open-Ended**
✅ Good: "What factors should be considered when..."

❌ Closed: "Should we do X? Yes or No?"

---

**5. Appropriate Difficulty**
Match the scenario complexity to:
- Participant background
- Available discussion time (typically 20-45 minutes)
- Training objectives

---

### Scenario Types

**1. Problem-Solving**
```
Example: "A school district wants to improve student engagement 
in remote learning. Design a comprehensive strategy considering 
technology access, teacher training, and student motivation."
```

**2. Ethical Dilemmas**
```
Example: "Your company can increase profits by 40% by moving 
production overseas, but this would eliminate 200 local jobs. 
What factors should guide this decision?"
```

**3. Analysis & Evaluation**
```
Example: "Three vendors have submitted proposals for your 
company's new software system. What criteria should you use 
to evaluate them beyond just price?"
```

**4. Innovation & Creativity**
```
Example: "Design a waste reduction program for a university 
campus that is both environmentally effective and financially 
sustainable within a limited budget."
```

**5. Case Studies**
```
Example: "A retail store's sales dropped 30% after a competitor 
opened nearby. Their prices are already the lowest in town. 
Identify alternative strategies to win back customers."
```

---

## ⚡ Quick Update Methods

### Scenario Template Library

**Copy and paste these ready-to-use scenarios:**

#### Business & Economics
```
1. Market Analysis: A startup gained 10,000 users but has zero 
   revenue. Develop a monetization strategy without losing users.

2. Strategic Planning: Your company must choose between expanding 
   to new markets or improving existing products. How would you 
   decide?

3. Crisis Management: A product recall has damaged your brand's 
   reputation. Design a recovery strategy.
```

#### Technology & Innovation
```
1. AI Ethics: An AI hiring tool shows bias against certain 
   demographics. Should it be fixed, paused, or discontinued? 
   Justify your decision.

2. Data Privacy: Balance user privacy with personalization in 
   a new app. What policies would you implement?

3. Digital Transformation: Help a traditional business adopt 
   digital tools while maintaining its core values.
```

#### Healthcare
```
1. Resource Allocation: A hospital has limited ICU beds during 
   a crisis. Develop fair criteria for patient prioritization.

2. Patient Care: Design a patient communication system that 
   works for all literacy levels and languages.

3. Preventive Care: Create a community health program with 
   limited funding. What would you prioritize?
```

#### Education
```
1. Curriculum Design: Develop a teaching method for students 
   with different learning speeds in one classroom.

2. Engagement Strategy: Student participation is low in online 
   classes. Propose solutions beyond mandatory attendance.

3. Assessment: Design a fair evaluation system that measures 
   both knowledge and critical thinking.
```

#### Environment & Sustainability
```
1. Climate Action: A city wants to reduce carbon emissions by 
   50% in 10 years. What sectors should they target first?

2. Sustainable Business: Make a manufacturing company carbon-
   neutral without significantly raising costs.

3. Conservation: Balance wildlife protection with local 
   community economic needs in a protected area.
```

---

## 🔄 Updating Scenarios for Different Sessions

### Scenario Rotation Strategy

**Week 1 Training:**
- Group 1: Business Problem A
- Group 2: Ethics Scenario A
- Group 3: Innovation Challenge A
- Group 4: Analysis Task A

**Week 2 Training:**
- Rotate all scenarios or introduce new ones
- Use the "Manage All Scenarios" feature
- Takes 2-3 minutes to update everything

---

### Theme-Based Scenarios

**All Healthcare Theme:**
```
Group 1: Hospital efficiency
Group 2: Medical ethics
Group 3: Patient experience innovation
Group 4: Healthcare policy analysis
```

**All Technology Theme:**
```
Group 1: Software development trade-offs
Group 2: AI ethics
Group 3: UX/UI problem solving
Group 4: Technology strategy
```

---

## 🛠️ Troubleshooting

### Issue: Scenarios Not Updating for New Participants

**Check:**
1. Did you click "Save" after editing?
2. Refresh the admin dashboard to verify changes
3. Check Firebase Console → scenarios node

**Fix:**
- Wait 5-10 seconds for Firebase to sync
- Clear browser cache
- Test with a new registration

---

### Issue: Scenarios Reset to Default

**Cause:** Scenarios weren't saved to Firebase, only existed in code

**Fix:**
1. Open Admin Dashboard
2. Use "Manage All Scenarios" to set them in Firebase
3. Once saved to Firebase, they persist forever

---

### Issue: Scenario Too Long on Mobile

**Check:** Test on mobile device or narrow browser window

**Fix:**
- Shorten to 2-4 sentences
- Remove unnecessary details
- Focus on core question/task

---

### Issue: Can't Access Scenario Editor

**Check:**
1. Are you on the admin dashboard?
2. Is Firebase configured correctly?
3. Check browser console for errors (F12)

**Fix:**
- Verify Firebase config is correct
- Check internet connection
- Try different browser

---

## 💡 Pro Tips

### 1. Prepare Scenarios in Advance
- Write all scenarios in a document first
- Review for clarity and balance
- Copy-paste into admin dashboard
- Test with one participant before sharing widely

---

### 2. Keep a Scenario Library
Create a document with your best scenarios by category:
```
📁 My Scenario Library
  ├── Business Scenarios
  ├── Ethics Scenarios
  ├── Innovation Scenarios
  └── Analysis Scenarios
```

---

### 3. Balance Difficulty
Ensure all four groups have similar difficulty levels:
- Don't make Group 1 much harder than Group 4
- Test scenarios with colleagues first
- Adjust based on participant feedback

---

### 4. Version Control
Keep track of what worked:
```
Session 1 (Jan 2026): Healthcare scenarios - Great engagement
Session 2 (Feb 2026): Business scenarios - Need more specificity
Session 3 (Mar 2026): Mixed topics - Participants preferred focused themes
```

---

### 5. Update During Registration
- Monitor registrations in real-time
- If groups are unbalanced (e.g., Group 1 has 10, Group 4 has 2)
- You can still update scenarios up until session starts
- No coding required!

---

## 📝 Quick Reference: Update Process

### One Scenario Update (30 seconds)
```
1. Open admin.html
2. Find the group card
3. Click "✏️ Edit"
4. Type new scenario
5. Click "💾 Save"
✅ Done!
```

### All Scenarios Update (2 minutes)
```
1. Open admin.html
2. Click "📝 Manage All Scenarios"
3. Edit all four text boxes
4. Click "💾 Save All Scenarios"
✅ Done!
```

### Via Firebase (Advanced, 1 minute)
```
1. Firebase Console → Realtime Database
2. Navigate to scenarios/
3. Click group1, group2, group3, or group4
4. Edit text directly
5. Press Enter
✅ Done!
```

---

## 🎓 Sample Workflow: Preparing for a New Training

**1 Week Before:**
- [ ] Decide on training theme
- [ ] Write 4 scenarios
- [ ] Review for clarity and balance

**3 Days Before:**
- [ ] Open admin dashboard
- [ ] Click "Manage All Scenarios"
- [ ] Paste all four scenarios
- [ ] Save changes

**1 Day Before:**
- [ ] Do a test registration
- [ ] Verify scenarios appear correctly
- [ ] Check mobile display

**Day Of:**
- [ ] Open admin dashboard
- [ ] Monitor registrations
- [ ] Export participant list before session
- [ ] Have scenarios ready for reference during activity

---

## ✅ Scenario Update Checklist

Before each training session:

- [ ] Scenarios are relevant to your audience
- [ ] All four scenarios are similar difficulty
- [ ] Scenarios are 2-4 sentences (mobile-friendly)
- [ ] Each scenario has a clear task/question
- [ ] Scenarios align with training objectives
- [ ] You've tested how they display (admin dashboard + test registration)
- [ ] Scenarios are saved in Firebase (not just in code)
- [ ] You have backup scenarios ready if needed

---

## 🎉 You're Ready!

Scenario management is designed to be **simple and flexible**. You can:
- ✅ Update scenarios anytime (even during registration)
- ✅ No coding or technical skills required
- ✅ Changes take effect immediately
- ✅ Scenarios persist between sessions
- ✅ Easy to create themed training sessions

**Remember:** The admin dashboard is your control center. Everything you need is there!

---

**Questions?** 
- See SETUP_GUIDE.md for Firebase basics
- See QUICK_REFERENCE.md for day-of-event tips
- See TECHNICAL_DOCS.md for advanced customization

**Happy Training!** 🧠
