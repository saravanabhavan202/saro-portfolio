🚀 Portfolio Setup & Deployment Guide
This guide will help you upload your portfolio to GitHub and deploy it online.
📋 Prerequisites
Before you begin, make sure you have:
·	A GitHub account (Sign up here)
·	Git installed on your computer (Download here)
·	All portfolio files in one folder
📁 Your Portfolio Files
Make sure you have these files in your portfolio folder:
portfolio/
├── portfolio.html
├── profile.jpeg
├── Saravanabhavan_Resume.pdf
├── README.md
└── .gitignore

🔧 Step-by-Step Setup
Step 1: Rename Your Main File
For GitHub Pages to work automatically, rename your HTML file:
# Rename portfolio.html to index.html
mv portfolio.html index.html

Step 2: Create a GitHub Repository
1.	Go to GitHub
2.	Click the "+" icon in the top right
3.	Select "New repository"
4.	Name it: portfolio (or any name you prefer)
5.	Keep it Public
6.	DON'T initialize with README (we already have one)
7.	Click "Create repository"
Step 3: Upload to GitHub
Open Terminal/Command Prompt in your portfolio folder and run:
# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial portfolio commit"

# Add your GitHub repository as remote
# Replace YOUR-USERNAME with your actual GitHub username
git remote add origin https://github.com/YOUR-USERNAME/portfolio.git

# Push to GitHub
git branch -M main
git push -u origin main

Step 4: Enable GitHub Pages
1.	Go to your repository on GitHub
2.	Click Settings (top menu)
3.	Scroll to Pages (left sidebar)
4.	Under Source, select:
1.	Branch: main
2.	Folder: / (root)
5.	Click Save
6.	Wait 1-2 minutes
7.	Your site will be live at: https://YOUR-USERNAME.github.io/portfolio/
✅ Verification Checklist
After deployment, verify:
·	Website loads correctly
·	Profile picture displays
·	Background image shows
·	Resume downloads properly
·	All project links work
·	Responsive on mobile
·	Social media links work
🔄 Making Updates
After making changes to your portfolio:
# Save your changes
git add .

# Commit with a message
git commit -m "Update: describe your changes here"

# Push to GitHub
git push origin main

Changes will be live in 1-2 minutes!
🌐 Custom Domain (Optional)
Want a custom domain like saravanabhavan.dev?
1.	
2.	Buy a domain from:
1.	Namecheap
2.	GoDaddy
3.	Google Domains
3.	
4.	In your repository settings > Pages:
1.	Enter your custom domain
2.	Save
5.	
6.	In your domain registrar, add these DNS records:
7.	Type: A
Host: @
Value: 185.199.108.153

Type: A
Host: @
Value: 185.199.109.153

Type: A
Host: @
Value: 185.199.110.153

Type: A
Host: @
Value: 185.199.111.153

Type: CNAME
Host: www
Value: YOUR-USERNAME.github.io

8.	
9.	Wait 24-48 hours for DNS to propagate
🐛 Troubleshooting
Issue: Website not loading
Solution:
·	Wait 2-3 minutes after enabling Pages
·	Check that index.html exists (not portfolio.html)
·	Verify repository is Public
Issue: Images not showing
Solution:
·	Make sure all images are in the repository
·	Check file names match exactly (case-sensitive)
·	Use relative paths, not absolute paths
Issue: Resume won't download
Solution:
·	Verify PDF file is uploaded
·	Check the file name matches in HTML
·	Make sure file size is under 100MB
Issue: Git push rejected
Solution:
git pull origin main --rebase
git push origin main

📊 Analytics (Optional)
Want to track visitors?
Google Analytics
1.	Go to Google Analytics
2.	Create account and property
3.	Get tracking code
4.	Add before </head> in index.html:
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>

🎯 Alternative Hosting Options
Netlify
1.	Go to Netlify
2.	Sign up with GitHub
3.	Click "New site from Git"
4.	Select your repository
5.	Click Deploy
Vercel
1.	Go to Vercel
2.	Sign up with GitHub
3.	Click "Import Project"
4.	Select your repository
5.	Click Deploy
📱 SEO Optimization
Add to <head> section in index.html:
<!-- SEO Meta Tags -->
<meta name="description" content="Saravanabhavan.S - Java Full Stack Developer Portfolio. Specialized in Spring Boot, React.js, and modern web technologies.">
<meta name="keywords" content="Java Developer, Full Stack Developer, Spring Boot, React.js, Web Development, Saravanabhavan">
<meta name="author" content="Saravanabhavan.S">

<!-- Open Graph for Social Media -->
<meta property="og:title" content="Saravanabhavan.S - Java Full Stack Developer">
<meta property="og:description" content="Portfolio showcasing web development projects and skills">
<meta property="og:image" content="profile.jpeg">
<meta property="og:url" content="https://YOUR-USERNAME.github.io/portfolio/">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Saravanabhavan.S - Portfolio">
<meta name="twitter:description" content="Java Full Stack Developer">
<meta name="twitter:image" content="profile.jpeg">

🎓 Next Steps
1.	
2.	Share your portfolio:
1.	Add link to LinkedIn profile
2.	Include in resume
3.	Share on social media
4.	Add to email signature
3.	
4.	Keep it updated:
1.	Add new projects
2.	Update skills
3.	Refresh resume
4.	Add blog posts
5.	
6.	Get feedback:
1.	Share with mentors
2.	Post on developer communities
3.	Ask for code reviews
💡 Pro Tips
·	✅ Update portfolio regularly (monthly)
·	✅ Add Google Analytics to track visitors
·	✅ Optimize images for faster loading
·	✅ Test on different devices
·	✅ Keep resume updated
·	✅ Link to live project demos
·	✅ Add case studies for major projects
·	✅ Include testimonials if available
📞 Need Help?
If you encounter issues:
1.	Check GitHub's Pages documentation
2.	Search on Stack Overflow
3.	Ask in developer communities
4.	Open an issue on your repository

Good luck with your portfolio! 🚀
Made with ❤️ by Saravanabhavan.S
