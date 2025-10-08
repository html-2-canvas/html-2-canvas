========================================
HTML2CANVAS WEBSITE - README
========================================

Welcome to your professional HTML2Canvas website! This multi-page website is built with HTML, CSS, and JavaScript, featuring a modern, responsive design.

========================================
FILE STRUCTURE
========================================

html2canvas5/
├── index.html          (Home page with hero section and features)
├── about.html          (About page with mission and vision)
├── contact.html        (Contact page with Google Form button)
├── download.html       (Download page with installation guide)
├── style.css           (All styling and responsive design)
├── script.js           (Interactive features and animations)
└── README.txt          (This file - setup instructions)

========================================
HOW TO RUN THE SITE LOCALLY
========================================

METHOD 1: Direct File Opening
1. Navigate to the project folder (html2canvas5)
2. Double-click on index.html to open in your default browser
3. Use the navigation menu to explore other pages

METHOD 2: Using a Local Server (Recommended)
If you have Python installed:
1. Open Command Prompt/Terminal in the project folder
2. Run: python -m http.server 8000
   (or: python3 -m http.server 8000)
3. Open browser and go to: http://localhost:8000

If you have Node.js installed:
1. Install http-server globally: npm install -g http-server
2. Navigate to project folder in terminal
3. Run: http-server
4. Open the URL shown in the terminal

Using VS Code Live Server:
1. Install "Live Server" extension in VS Code
2. Right-click on index.html
3. Select "Open with Live Server"

========================================
CUSTOMIZATION GUIDE
========================================

--- CHANGING COLORS ---

The website uses a consistent color palette defined in style.css:

Primary Color (Coral/Orange): #FF7757
Secondary Color (Light Peach): #FFEEEA
Accent Color (Dark Blue-Gray): #404757
White: #FFFFFF

To change colors:
1. Open style.css
2. Find the :root section at the top (lines 9-17)
3. Modify the CSS variables:
   --primary-color: #FF7757;     (Main action color)
   --secondary-color: #FFEEEA;   (Background highlights)
   --accent-color: #404757;      (Text and dark elements)
   --white: #FFFFFF;             (Main background)

These colors will automatically update throughout the entire website.

--- CHANGING TEXT CONTENT ---

Home Page (index.html):
- Hero Title: Line 41-42
- Hero Description: Line 43-46
- Feature Cards: Lines 65-90
- Content Sections: Lines 96-155

About Page (about.html):
- Page Header: Lines 31-33
- Mission/Vision Cards: Lines 42-80
- Story Content: Lines 89-105
- Statistics: Lines 113-132

Contact Page (contact.html):
- Page Header: Lines 31-33
- Contact Description: Lines 38-43
- Contact Info Items: Lines 49-78
- Form Button Text: Line 90

Download Page (download.html):
- Page Header: Lines 31-33
- Download Features: Lines 51-66
- Installation Commands: Lines 107-135
- Quick Start Steps: Lines 147-184

--- REPLACING LINKS ---

Google Form Link (contact.html):
Line 86: Replace the href URL with your Google Form link
Current: https://docs.google.com/forms/d/e/1FAIpQLSelru1QfiYeo1ScnG7zA_OsaqxsBXICobniMKvsCVNxsOTtYw/viewform?usp=header

GitHub Repository Link:
Replace in ALL files (navigation):
Current: https://github.com/html-2-canvas/html2canvas
Find in: Lines with class "github-link"

Download Link (download.html):
Line 70: Replace the href URL
Current: https://html2canvas.net/download/

Official Site Link:
Replace: https://html2canvas.net/
Found throughout all pages in various buttons and links

--- CHANGING FONTS ---

Current font: Poppins (from Google Fonts)

To change the font:
1. Visit Google Fonts: https://fonts.google.com
2. Select your desired font
3. Copy the <link> tag provided
4. Replace the font link in ALL HTML files (in <head> section)
5. Update style.css, line 22:
   font-family: 'YourFontName', sans-serif;

Popular alternatives:
- Inter: Modern, clean, professional
- Roboto: Versatile, widely used
- Montserrat: Geometric, modern
- Open Sans: Friendly, readable

--- ADDING/REMOVING PAGES ---

To add a new page:
1. Create a new HTML file (e.g., services.html)
2. Copy the structure from any existing page
3. Add navigation link to ALL pages:
   <li><a href="services.html">Services</a></li>
4. Update footer links in all pages

To remove a page:
1. Delete the HTML file
2. Remove navigation links from ALL pages
3. Remove footer links from ALL pages

--- MODIFYING FOOTER ---

Footer content is at the bottom of each HTML file.

Brand Name: Line with <h3>HTML2Canvas</h3>
Copyright Year: Line with &copy; 2024
Designer Credit: "Designed & Developed with ❤️ by..."

To update:
1. Change text in each HTML file's footer section
2. Or use search & replace across all files

--- CUSTOMIZING KEYWORDS AND SEO ---

Focus Keywords are integrated in index.html:
- "npm html2canvas" - Line 85 (linked to main site)
- "html2canvas options" - Line 102 (linked to alternatives page)
- "javascript resize image base64" - Line 119 (linked to conversion guide)

To change keywords:
1. Update the text naturally within paragraphs
2. Update the href links to match your target URLs
3. Update meta descriptions in <head> of each page

========================================
RESPONSIVE DESIGN
========================================

The website is fully responsive with breakpoints:
- Desktop: 1200px and above
- Tablet: 768px - 1199px
- Mobile: Below 768px

To modify responsive behavior:
1. Open style.css
2. Find @media queries at the bottom (starting line ~1090)
3. Adjust breakpoints or add new ones

========================================
INTERACTIVE FEATURES
========================================

Mobile Navigation:
- Hamburger menu appears below 768px width
- Toggle functionality in script.js

Smooth Scrolling:
- Scroll animations for cards and sections
- Fade-in effects on scroll

Copy to Clipboard:
- Code blocks on download page have copy buttons
- Implemented in script.js (copyCode function)

Auto-hide Navigation:
- Navbar hides when scrolling down
- Reappears when scrolling up

========================================
BROWSER COMPATIBILITY
========================================

Tested and compatible with:
✓ Chrome (latest)
✓ Firefox (latest)
✓ Safari (latest)
✓ Edge (latest)
✓ Mobile browsers (iOS Safari, Chrome Mobile)

========================================
PERFORMANCE OPTIMIZATION
========================================

Tips for better performance:
1. Optimize images before adding them
2. Use WebP format for better compression
3. Minimize custom fonts (currently using only Poppins)
4. Keep CSS and JS files linked externally (already done)
5. Enable browser caching if hosting on a server

========================================
TROUBLESHOOTING
========================================

Issue: Google Form button doesn't work
Solution: Make sure pop-ups are enabled in browser settings

Issue: Mobile menu not working
Solution: Check that script.js is properly linked in HTML files

Issue: Colors not changing
Solution: Clear browser cache (Ctrl+Shift+Delete) and refresh

Issue: Fonts not loading
Solution: Check internet connection (Google Fonts requires internet)

Issue: Layout breaks on mobile
Solution: Ensure viewport meta tag is present in HTML <head>

========================================
DEPLOYMENT OPTIONS
========================================

Option 1: GitHub Pages (Free)
1. Create a GitHub repository
2. Upload all files
3. Go to Settings > Pages
4. Select main branch as source
5. Your site will be live at: username.github.io/repository-name

Option 2: Netlify (Free)
1. Visit netlify.com
2. Drag and drop your project folder
3. Site goes live instantly
4. Get a free subdomain or connect custom domain

Option 3: Vercel (Free)
1. Visit vercel.com
2. Import from GitHub or upload files
3. Deploy with one click
4. Get instant HTTPS

Option 4: Traditional Web Hosting
1. Choose a hosting provider (Hostinger, Bluehost, etc.)
2. Upload files via FTP/cPanel
3. Set index.html as the default page

========================================
SUPPORT AND RESOURCES
========================================

HTML Documentation: https://developer.mozilla.org/en-US/docs/Web/HTML
CSS Documentation: https://developer.mozilla.org/en-US/docs/Web/CSS
JavaScript Documentation: https://developer.mozilla.org/en-US/docs/Web/JavaScript

Google Fonts: https://fonts.google.com
Color Palette Tools: https://coolors.co
Icon Resources: https://heroicons.com

========================================
LICENSE & CREDITS
========================================

This website template is provided as-is for your use.
Feel free to modify, customize, and deploy as needed.

Technologies Used:
- HTML5 for structure
- CSS3 for styling and animations
- JavaScript (Vanilla) for interactivity
- Google Fonts (Poppins)

Design Inspired by: html2canvas.net
Custom developed with modern best practices

========================================
VERSION HISTORY
========================================

Version 1.0 (2024)
- Initial release
- 4 responsive pages
- Modern design with color palette
- Mobile-friendly navigation
- Smooth animations
- Copy-to-clipboard functionality

========================================
FINAL NOTES
========================================

Thank you for using this website template! 

For best results:
✓ Keep content concise and relevant
✓ Optimize images before adding
✓ Test on multiple devices
✓ Update links to match your actual resources
✓ Customize colors to match your brand
✓ Keep the design clean and professional

If you make changes to the HTML structure, ensure all pages maintain consistency in navigation and footer elements.

Happy customizing! 🚀

========================================
