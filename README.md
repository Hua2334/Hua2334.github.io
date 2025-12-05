# Amber Wang's Personal Homepage

A responsive personal portfolio website built with HTML, CSS, and vanilla JavaScript.

## 🚀 Features

- **About Section**: Personal introduction with profile information
- **Skills Tag Cloud**: Interactive skill tags with hover animations
- **Experience Timeline**: Chronological display of achievements and milestones
- **Portfolio Projects**: Card-based project showcase with detail pages
- **Progress Bar**: Visual scroll indicator with clickable section markers
- **Responsive Design**: Fully responsive layout for mobile, tablet, and desktop
- **Accessibility**: Keyboard navigation, ARIA labels, and semantic HTML

## 📁 Project Structure

```
.
├── index.html          # Main homepage
├── styles.css          # Global styles and responsive breakpoints
├── projects/           # Individual project detail pages
│   ├── project1.html
│   ├── project2.html
│   ├── project3.html
│   └── project4.html
├── README.md           # This file
└── help.txt            # Local testing instructions
```

## 🛠️ Technologies Used

- HTML5 (Semantic markup)
- CSS3 (Grid, Flexbox, CSS Variables)
- Vanilla JavaScript (No external dependencies)
- Responsive design (Mobile-first approach)

## 🌐 Local Testing

```bash
# Start local development server
cd /Users/amber/Desktop/MyApp/Hua2334.github.io
python3 -m http.server 8000

# Open in browser
http://localhost:8000/
```

## 📊 Git Workflow & Version Control

### Main Branches
- **main**: Production-ready code
- **feature/skills-tags**: Feature branch with enhancements

### Meaningful Commits

This project demonstrates professional git practices with clear, atomic commits:

1. **feat: enhance Experience section with detailed descriptions** (57d9b0e)
   - Added event descriptions for timeline items (2019, 2024, 2025)
   - Implemented `.event-desc` styling with italic font and improved readability

2. **feat: improve progress bar marker accessibility** (1e88930)
   - Added `aria-label` attributes to progress markers for screen readers
   - Implemented keyboard navigation support (Enter/Space keys)
   - Set `tabindex='0'` to make markers keyboard focusable

3. **style: refine responsive design and accessibility** (29de831)
   - Added focus styles to progress markers for keyboard navigation
   - Optimized event description font size on mobile devices
   - Enhanced spacing and readability in timeline on screens < 600px

4. **fix: restore event descriptions in timeline** (0e46daa)
   - Restored accidentally removed event descriptions

5. **Merge PR** (7de85f3)
   - Merged feature/skills-tags branch into main with comprehensive description

### Version Control Notes

#### 🔄 Git Revert Operation

**Commit**: f8f14f2  
**Message**: Revert "style: refine responsive design and accessibility"

**Reason for Revert**:
We reverted commit 29de831 to demonstrate the importance of version control and the ability to safely undo changes while maintaining a clear audit trail. This revert shows that:
- Progress markers focus styles (added in commit 29de831) needed refinement
- Mobile optimization should be handled separately in a dedicated commit
- Using `git revert` (vs `git reset`) preserves all history for accountability

**Resolution**: The reverted changes will be incorporated back into feature/A as an improved implementation in the next iteration.

---

## 📋 A/B Testing: Feature Variants

This project includes two feature branch variants exploring different UI/UX approaches:

### Feature/A: Enhanced Timeline with Collapsible Details
- **Branch**: `feature/A`
- **Approach**: 
  - Experience timeline items are collapsible with expand/collapse buttons
  - Each timeline event shows a brief description with a "Read more" link
  - Smooth animations when expanding/collapsing content
  - Better mobile space utilization by hiding detailed descriptions initially

- **Pros**:
  - ✅ Better mobile performance (less initial content to render)
  - ✅ Cleaner visual hierarchy (users focus on main events first)
  - ✅ Interactive elements provide better engagement
  
- **Cons**:
  - ❌ Extra JavaScript required for collapse/expand logic
  - ❌ Users must click to see full descriptions (may miss context)

### Feature/B: Expanded Timeline with Full Inline Descriptions
- **Branch**: `feature/B`
- **Approach**:
  - All timeline descriptions are displayed inline without collapsing
  - Horizontal timeline on desktop, vertical on mobile
  - Descriptions styled with color-coded badges per year
  - Timeline markers use icons to indicate event type (swimming, sports, competition)

- **Pros**:
  - ✅ All information visible at once (no hidden content)
  - ✅ Simpler implementation (minimal JavaScript)
  - ✅ Better for SEO (all text content is discoverable)
  
- **Cons**:
  - ❌ Mobile experience is cramped (too much vertical scrolling)
  - ❌ Overwhelming visual density on small screens

### Decision: Adopting Feature/A

**Why Feature/A was chosen:**
- Better mobile UX with progressive disclosure pattern
- Users can quickly scan main events then click for details
- Aligns with modern web standards (collapsible content is familiar)
- Improved performance on mobile devices with large timeline content

**Why Feature/B was not chosen:**
- Mobile layout becomes cluttered with full descriptions
- Users on mobile may experience fatigue from excessive scrolling
- Feature/B can be reconsidered if user feedback suggests always-visible descriptions are preferred

**Status**:
- ✅ Feature/A: Merged to main (PR #1)
- ❌ Feature/B: Kept as reference (PR #2 open but not merged)

---

## 📝 Development Notes

### Responsive Breakpoints
- **Desktop** (> 900px): 3-column portfolio grid, horizontal timeline
- **Tablet** (600px - 900px): 2-column portfolio grid, horizontal timeline
- **Mobile** (< 600px): Single column layout, vertical timeline, optimized spacing

### Accessibility Features
- Keyboard navigation support on progress bar markers
- ARIA labels for screen readers
- Semantic HTML5 structure
- Focus visible styles for keyboard users
- Color contrast compliant with WCAG guidelines

### Browser Compatibility
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📞 Contact

Email: [414570576@m365.fju.edu.tw](mailto:414570576@m365.fju.edu.tw)  
Instagram: [@chyl.07_](https://instagram.com/chyl.07_)

---

**Last Updated**: 2025-12-05  
**Branch**: main  
**Status**: Production Ready