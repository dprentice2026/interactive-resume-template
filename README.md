# Interactive Resume Template

A modern, responsive HTML resume template featuring an interactive design with smooth navigation, print-to-PDF capability, and project filtering. Perfect for professionals looking to create an engaging, professionally-designed resume that stands out.

## Features

✨ **Modern Design**
- Clean, professional aesthetic with a gradient background
- Responsive layout that works on desktop, tablet, and mobile
- Smooth animations and transitions

🎯 **Interactive Elements**
- Sticky navigation bar with smooth scrolling
- Project category filtering
- Clickable role buttons for quick navigation
- Print/PDF export functionality

🔍 **Recruiter-Friendly**
- Fast scanning with clear section hierarchy
- Accessibility features (ARIA labels, focus states)
- Optimized print styling for PDF export
- SEO-friendly HTML structure

## Getting Started

### 1. Open the Template
1. Download or clone this repository
2. Open `interactive_resume_template.html` in your web browser
3. The file will render immediately with placeholder content

### 2. Edit Your Information
Replace all `[PLACEHOLDER TEXT]` sections with your actual information:

#### Header Section
- `[YOUR FULL NAME]` - Your name (appears in title and page header)
- `[YOUR CITY, STATE]` - Your location
- `[JOB TITLE 1/2/3]` - Your professional roles (up to 3 buttons)
- Contact links: Email, phone, LinkedIn, GitHub, Portfolio

#### Summary Section
- `[Add your professional summary...]` - 2-3 sentences about your background and goals

#### Skills Section
- `[SKILL CATEGORY 1/2/3/4]` - Organize skills by category
- `[Skill 1/2/3...]` - Individual skills within each category
- Current Development Focus - What you're learning or working on

#### Experience Section
- `[JOB TITLE]` - Your position
- `[Company Name] | [Location] | [Start Date] - [End Date]` - Employment details
- Bullet points - Key achievements and responsibilities

#### Projects Section
- `[PROJECT NAME]` - Project title
- `[Project Type/Technology]` - What kind of project (e.g., "Web Application", "Design File")
- Project details and accomplishment
- `[PROJECT LINK]` - Link to live project, repository, or portfolio piece

#### Education Section
- `[SCHOOL/UNIVERSITY NAME]` - Institution name
- `[Degree Type] in [Field of Study]` - Degree information
- GPA and graduation date
- Relevant coursework or areas of study

## Customization Guide

### Changing Colors
The template uses CSS custom properties (variables) for easy color customization. Edit the `:root` section in the `<style>` tag:

```css
:root {
  --bg-0: #f3f7fa;           /* Primary background */
  --bg-1: #e8eff5;           /* Secondary background */
  --accent: #0f6ba8;         /* Primary accent color */
  --accent-2: #005f73;       /* Secondary accent color */
  --focus: #f59e0b;          /* Focus/highlight color */
  --ok: #2f855a;             /* Success color */
  /* ... other variables ... */
}
```

### Adding More Sections
To add a new section (e.g., "Awards", "Publications"):

1. Create a new card block:
```html
<section class="card" id="awards">
  <div class="card-inner">
    <div class="section-head">
      <h2>Awards & Recognition</h2>
    </div>
    <!-- Your content here -->
  </div>
</section>
```

2. Add navigation link in the topbar:
```html
<a class="nav-btn" href="#awards">Awards</a>
```

### Adding More Projects
Each project in the portfolio follows this structure:

```html
<article class="project" data-tags="category1 category2">
  <h3>[PROJECT NAME]</h3>
  <p class="exp-meta">[Project Type]</p>
  <ul class="list">
    <li>[Detail 1]</li>
    <li>[Detail 2]</li>
  </ul>
  <p><a href="[LINK]" target="_blank" rel="noopener noreferrer">View Project</a></p>
</article>
```

**Project Tags:**
- Use `data-tags="tag1 tag2"` to assign projects to categories for filtering
- Categories are automatically created based on tags you use
- Update filter buttons to match your categories

### Modifying Filter Categories
To change project filter categories, update both the filter buttons and project tags:

1. Change button names:
```html
<button class="filter-btn" type="button" data-filter="design">Design</button>
```

2. Assign matching tags to projects:
```html
<article class="project" data-tags="design">
```

## Using the Template

### Viewing Your Resume
1. Open the HTML file in your web browser
2. Use the sticky navigation bar to jump between sections
3. Click role buttons to navigate to specific sections
4. Use project filters to display only certain project categories

### Printing/Saving as PDF
1. Click the **Print/PDF** button in the top right corner
2. In the print dialog, select:
   - Destination: "Save as PDF" (or your preferred printer)
   - Paper size: Letter
   - Margins: Default (0.45in)
   - Uncheck "Headers and footers"
3. Click **Save** or **Print**

### Sharing Your Resume
- **As HTML:** Share the `.html` file directly (works in any web browser)
- **As PDF:** Use the Print/PDF function to create a PDF version
- **On Web:** Upload the HTML file to a web server and share the URL
- **On GitHub:** Commit to your repository and enable GitHub Pages

## Tips for Best Results

✅ **DO:**
- Keep your professional summary concise (2-3 sentences)
- Use specific achievements with quantifiable results when possible
- Include links to live projects, code repositories, or portfolio pieces
- Regularly update your resume with new projects and skills
- Test printing in different browsers to ensure formatting looks good

❌ **DON'T:**
- Overload a single section with too much text
- Use more than 3 professional titles in the role row
- Include outdated information or projects you're not proud of
- Use placeholder text in the final version
- Forget to test the Print/PDF function before sending

## Browser Support

This template works best in modern browsers:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Accessibility

The template includes:
- Semantic HTML structure
- ARIA labels for navigation and interactive elements
- Keyboard-navigable links and buttons
- Focus-visible states for accessibility
- Readable color contrast ratios

## Responsive Design

The template automatically adjusts for different screen sizes:
- **Desktop (1000px+):** Full two-column layout
- **Tablet (761-999px):** Single column with adjusted spacing
- **Mobile (≤760px):** Optimized single-column layout with centered navigation

## Troubleshooting

**Issue:** Links not working  
**Solution:** Make sure your URLs include the full protocol (e.g., `https://` or `mailto:`)

**Issue:** Print/PDF looks different than on screen  
**Solution:** The template has special print-only CSS. Check the print preview and adjust margins if needed.

**Issue:** Colors not displaying correctly  
**Solution:** Clear your browser cache and reload the file

**Issue:** Navigation isn't sticky on mobile  
**Solution:** This is intentional for mobile space optimization. You can scroll the navbar on small screens.

## File Structure

```
interactive_resume_template.html    Main template file (this is all you need!)
README.md                          Documentation (this file)
```

## Customizing for Your Field

The template is versatile and works for many professions:

- **Software Developer:** Use for tech skills, GitHub projects, open-source contributions
- **Designer:** Showcase design work, Figma files, portfolio links
- **Project Manager:** Highlight leadership, achievements, certifications
- **Data Scientist:** Feature data projects, research, visualizations
- **Creative Professional:** Display portfolio, side projects, creative work

Simply adapt the section names and content to match your industry!

## Tips for Different Industries

### Tech/Engineering
- Include GitHub profile link
- Showcase open-source contributions
- Link to live demos or deployed projects
- Highlight programming languages and frameworks

### Design
- Include Figma profile or design portfolio
- Link to case studies or project showcases
- Add links to Behance, Dribbble, or personal site
- Showcase visual projects

### Business/Management
- Emphasize quantifiable achievements (revenue, team size, etc.)
- Highlight leadership and soft skills
- Include relevant certifications
- Focus on results and business impact

## Legal & License

This template is free to use and modify for personal and professional purposes. Feel free to share it with others and customize it as needed.

## Questions or Feedback?

If you have questions about using this template or suggestions for improvement, consider:
- Creating an issue in the repository
- Reaching out to the template creator
- Customizing it further to match your needs

---

**Happy resume building!** 🚀

Make your resume stand out and showcase your professional journey in an engaging, interactive way.
