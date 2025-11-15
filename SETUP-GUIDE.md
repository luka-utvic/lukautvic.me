# Complete Guide: Setting Up Your Personal Website with Namecheap & GitHub Pages

**A Student's Step-by-Step Guide to Getting Your Website Live with HTTPS**

By Luka Utvic | University of Illinois Chicago

---

## Table of Contents
1. [Prerequisites](#prerequisites)
2. [Part 1: Register Your Domain with Namecheap](#part-1-register-your-domain-with-namecheap)
3. [Part 2: Set Up GitHub Repository](#part-2-set-up-github-repository)
4. [Part 3: Create Your Website](#part-3-create-your-website)
5. [Part 4: Enable GitHub Pages](#part-4-enable-github-pages)
6. [Part 5: Connect Your Custom Domain](#part-5-connect-your-custom-domain)
7. [Part 6: Enable HTTPS](#part-6-enable-https)
8. [Troubleshooting](#troubleshooting)
9. [Tips & Best Practices](#tips--best-practices)

---

## Prerequisites

Before you start, you'll need:
- A GitHub account (free) - [Sign up here](https://github.com/join)
- Basic text editing skills
- About 30-60 minutes of time

- **Note** if you are feeling stuck, don't be afriad to take advantage of AI tools. Copy and paste instructions you don't understand or take screenshots and insert them and ask for help. I knew nothing about any of this before starting and I used AI to help me through.
- If AI is giving you a hard time or you just need someone to help feel free to contact me using any of my links, phone number, or email!

- My [LinkedIN](www.linkedin.com/in/lukautvic)
- My Email: lukautvic07@gmail.com
- My Phone #: +1 224-409-3527

Total Cost: **FREE!**

---

## Part 1: Register Your Domain with Namecheap

### Step 1.1: Find Your Domain

1. Go to [Namecheap.com](https://www.namecheap.com) For Students go to [Namecheap for Education](https://www.nc.me)
2. In the search bar, type your desired domain name (e.g., "yourname")
3. Click the search button

**Pro Tips:**
- `.me` domains are great for personal sites (e.g., `lukautvic.me`)
- `.com` is classic and professional (.me is the only free option, should be just fine for what we are doing)
- Keep it short and memorable

### Step 1.2: Purchase/Claim Your Domain

1. Choose your desired domain in the search results 
2. Click "Add to Cart" next to your chosen domain
3. Review your cart (you can usually skip the extras like WhoisGuard for now)
4. Click "Confirm Order"
5. Create a Namecheap account or log in (Use school email!!)
6. Complete the payment (Free unless you choose not to use a .me one)

**Important:** Save your Namecheap login credentials securely!

### Step 1.3: Access Domain Management

1. After purchase, go to your [Namecheap Dashboard](https://ap.www.namecheap.com/dashboard)
2. Click on "Domain List" in the left sidebar
3. Find your domain and click "Manage"

**Don't configure DNS yet** - we'll do that in Part 5 after setting up GitHub Pages.

---

## Part 2: Set Up GitHub Repository

### Step 2.1: Create a New Repository

1. Log in to [GitHub](https://github.com)
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Configure your repository:
   - **Repository name:** `yourdomain.com` (e.g., `lukautvic.me`)
   - **Description:** "My personal website" (optional but recommended)
   - **Public:** Select "Public" (required for free GitHub Pages)
   - **Initialize with README:** Check this box
5. Click "Create repository"

### Step 2.2: Repository Created!

You now have a repository at: `https://github.com/YOUR-USERNAME/yourdomain.com`

---

## Part 3: Create Your Website

### Step 3.1: Create Your index.html File

1. In your repository, click "Add file" → "Create new file"
2. Name it: `index.html`
3. Add your HTML content (here's a starter template):

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Name - Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }
        .container {
            max-width: 800px;
            margin: 50px auto;
            padding: 40px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.2);
        }
        h1 {
            color: #333;
            margin-bottom: 10px;
        }
        .subtitle {
            color: #666;
            margin-bottom: 30px;
        }
        .section {
            margin: 30px 0;
        }
        .section h2 {
            color: #667eea;
            border-bottom: 2px solid #667eea;
            padding-bottom: 10px;
            margin-bottom: 15px;
        }
        .contact-links {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }
        .contact-links a {
            padding: 10px 20px;
            background: #667eea;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: background 0.3s;
        }
        .contact-links a:hover {
            background: #764ba2;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Your Name</h1>
        <p class="subtitle">Student at Your University</p>
        
        <div class="section">
            <h2>About Me</h2>
            <p>Write a brief introduction about yourself, your interests, and what you're studying.</p>
        </div>
        
        <div class="section">
            <h2>Education</h2>
            <p><strong>Your University</strong> - Your Major<br>
            Expected Graduation: Month Year</p>
        </div>
        
        <div class="section">
            <h2>Contact</h2>
            <div class="contact-links">
                <a href="mailto:your.email@example.com">Email</a>
                <a href="https://linkedin.com/in/yourprofile" target="_blank">LinkedIn</a>
                <a href="https://github.com/yourusername" target="_blank">GitHub</a>
            </div>
        </div>
    </div>
</body>
</html>
```

4. Scroll down and click "Commit changes"
5. Add a commit message like "Create homepage"
6. Click "Commit changes" again

### Step 3.2: Verify Your File

Your `index.html` file should now be visible in your repository!

---

## Part 4: Enable GitHub Pages

### Step 4.1: Access Repository Settings

1. In your GitHub repository, click the "Settings" tab (at the top)
2. Scroll down the left sidebar and click "Pages" (under "Code and automation")

### Step 4.2: Configure GitHub Pages

1. Under "Source", select the dropdown and choose: **Deploy from a branch**
2. Under "Branch":
   - Select **main** from the first dropdown
   - Select **/ (root)** from the second dropdown
3. Click **Save**

### Step 4.3: Wait for Deployment

1. GitHub will start building your site (this takes 1-3 minutes)
2. Refresh the page after a minute
3. You'll see a message: "Your site is live at https://YOUR-USERNAME.github.io/yourdomain.com/"
4. Click the link to view your site!

**Checkpoint:** Your website should now be live on GitHub Pages (though not yet on your custom domain).

---

## Part 5: Connect Your Custom Domain

### Step 5.1: Add Custom Domain in GitHub

1. Still on the GitHub Pages settings page
2. Under "Custom domain", type your domain: `yourdomain.com` (e.g., `lukautvic.me`)
3. Click **Save**
4. **IMPORTANT:** You'll see an error "DNS check unsuccessful" - this is normal! We need to configure Namecheap first.

### Step 5.2: Configure DNS in Namecheap

Now we connect your domain to GitHub:

1. Go to [Namecheap Dashboard](https://ap.www.namecheap.com/dashboard)
2. Click "Domain List" in the left sidebar
3. Find your domain and click "Manage"
4. Click the "Advanced DNS" tab

### Step 5.3: Add DNS Records

You need to add specific records. Click "Add New Record" and create these **FOUR A Records**:

**Record Type:** A Record  
**Host:** @  
**Value/IP Address:** `185.199.108.153`  
**TTL:** Automatic (or 30 min)

Click "Add New Record" again and add three more A Records with the same Host (@) but these IP addresses:
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

**Then add a CNAME Record:**

**Record Type:** CNAME Record  
**Host:** www  
**Value:** `YOUR-USERNAME.github.io.` (Replace YOUR-USERNAME with your actual GitHub username. **Don't forget the period at the end!**)  
**TTL:** Automatic (or 30 min)

### Step 5.4: Save and Wait

1. Click the green checkmark to save each record
2. **DNS propagation takes 10-30 minutes** (sometimes up to 48 hours, but usually much faster)
3. Grab a coffee or work on your website content while you wait!

### Step 5.5: Verify DNS in GitHub

1. Go back to your GitHub repository → Settings → Pages
2. Wait 10-30 minutes, then refresh the page
3. The "DNS check unsuccessful" error should change to a green "DNS check successful" ✓
4. Your domain should now be connected!

---

## Part 6: Enable HTTPS

### Step 6.1: Enable HTTPS in GitHub

1. Still in GitHub Settings → Pages
2. Under "Custom domain", you should see your domain with "DNS check successful"
3. Check the box that says: **"Enforce HTTPS"**
   - **Note:** This option may be grayed out initially. If so, wait 5-10 more minutes for GitHub to issue your SSL certificate.
4. Once enabled, your site will ONLY be accessible via `https://yourdomain.com`

### Step 6.2: Verify HTTPS

1. Open a new browser tab
2. Go to `https://yourdomain.com`
3. Look for the padlock icon 🔒 in the address bar - that means your site is secure!
4. Also try `http://yourdomain.com` - it should automatically redirect to HTTPS

**🎉 Congratulations! Your website is now live with HTTPS security!**

---

## Troubleshooting

### Problem: "DNS check unsuccessful" won't go away

**Solutions:**
- Wait longer (DNS can take up to 48 hours, though usually 30 minutes)
- Verify you entered the correct IP addresses in Namecheap
- Make sure the CNAME record ends with a period: `username.github.io.`
- Clear your browser cache and try again
- Use [WhatsMyDNS.net](https://whatsmydns.net) to check if DNS has propagated globally

### Problem: "Enforce HTTPS" is grayed out

**Solutions:**
- Wait 10-30 minutes after DNS check succeeds
- Make sure "DNS check successful" shows in GitHub
- Refresh the GitHub Pages settings page
- Try unchecking and rechecking the custom domain, then save again

### Problem: Website shows 404 error

**Solutions:**
- Make sure your file is named exactly `index.html` (lowercase)
- Verify the file is in the root directory (not in a folder)
- Check that GitHub Pages is enabled and deploying from the "main" branch
- Wait a few minutes after making changes - GitHub needs time to rebuild

### Problem: Changes aren't showing up

**Solutions:**
- Wait 1-3 minutes for GitHub to rebuild your site
- Clear your browser cache (Ctrl+Shift+Delete on Windows, Cmd+Shift+Delete on Mac)
- Try opening in an incognito/private window
- Hard refresh the page (Ctrl+F5 on Windows, Cmd+Shift+R on Mac)

### Problem: "www.yourdomain.com" doesn't work

**Solutions:**
- Make sure you added the CNAME record for "www" in Namecheap
- Verify the CNAME points to `username.github.io.` (with the period!)
- Wait for DNS propagation (10-30 minutes)

---

## Tips & Best Practices

### For Your Website

1. **Mobile Responsive:** Always include this in your `<head>`:
   ```html
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   ```

2. **Update Regularly:** Keep your portfolio current with new projects and experiences

3. **Professional Email:** Use a professional email address, not "partyguy420@email.com"

4. **Fast Loading:** Keep images optimized (use tools like TinyPNG.com)

5. **Add Analytics:** Consider Google Analytics to see who visits your site

### For Development

1. **Test Locally:** You can test your HTML files by opening them directly in your browser before committing

2. **Use Browser DevTools:** Press F12 to inspect and debug your website

3. **Version Control:** GitHub automatically saves every version - you can always go back if something breaks

4. **Learn Git:** Eventually learn to use Git on your computer for easier development

### For Security

1. **Keep Login Credentials Safe:** Use a password manager for Namecheap and GitHub

2. **Enable 2FA:** Turn on two-factor authentication for your GitHub account

3. **Regular Backups:** Download your repository occasionally as a backup

### Cost Saving Tips

1. **Domain Renewals:** Set a calendar reminder before your domain expires to renew or transfer

2. **Renewal Pricing:** First-year domain prices are often discounted; renewal prices may be higher

3. **GitHub Student Pack:** If you're a student, get the [GitHub Student Developer Pack](https://education.github.com/pack) for tons of free tools and credits!

---

## What's Next?

### Enhance Your Website

- Add more pages (About, Projects, Blog, etc.)
- Learn CSS to make it look better
- Learn JavaScript to add interactivity
- Use a framework like Bootstrap or Tailwind CSS
- Add a contact form using Formspree or similar service

### Advanced Topics

- Set up a blog with Jekyll (GitHub Pages supports it!)
- Use a custom 404 page
- Add Google Analytics
- Implement SEO best practices
- Create a portfolio showcase

### Resources for Learning

- [W3Schools](https://www.w3schools.com/) - HTML, CSS, JavaScript tutorials
- [MDN Web Docs](https://developer.mozilla.org/) - Comprehensive web development documentation
- [freeCodeCamp](https://www.freecodecamp.org/) - Free coding courses
- [GitHub Pages Documentation](https://docs.github.com/en/pages) - Official docs
- [CSS-Tricks](https://css-tricks.com/) - CSS tips and tricks

---

## Summary Checklist

- [ ] Purchased domain from Namecheap
- [ ] Created GitHub account
- [ ] Created public repository named after your domain
- [ ] Created index.html file
- [ ] Enabled GitHub Pages in repository settings
- [ ] Added custom domain in GitHub Pages settings
- [ ] Configured A records in Namecheap DNS (4 IP addresses)
- [ ] Configured CNAME record in Namecheap DNS (www subdomain)
- [ ] Waited for DNS propagation (10-30 minutes)
- [ ] Verified "DNS check successful" in GitHub
- [ ] Enabled "Enforce HTTPS" in GitHub Pages
- [ ] Verified site loads with HTTPS (padlock icon)
- [ ] Tested both yourdomain.com and www.yourdomain.com

---

## Need Help?

If you get stuck:

1. **Check the Troubleshooting section above**
2. **Search GitHub Community:** [GitHub Community](https://github.community/)
3. **Namecheap Support:** They have 24/7 live chat
4. **Ask Your Fellow Students:** Share this guide and help each other!
5. **Stack Overflow:** Search for your specific error message

---

**Good luck with your website! 🚀**

*Created by Luka Utvic - Feel free to share this guide with other students!*

---

## Appendix: DNS Record Reference

For quick reference, here are the exact DNS records you need:

### A Records (Add all 4)
| Type | Host | Value | TTL |
|------|------|-------|-----|
| A | @ | 185.199.108.153 | Automatic |
| A | @ | 185.199.109.153 | Automatic |
| A | @ | 185.199.110.153 | Automatic |
| A | @ | 185.199.111.153 | Automatic |

### CNAME Record
| Type | Host | Value | TTL |
|------|------|-------|-----|
| CNAME | www | YOUR-USERNAME.github.io. | Automatic |

*Remember to replace YOUR-USERNAME with your actual GitHub username and don't forget the period at the end of the CNAME value!*
