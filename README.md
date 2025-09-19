# ToothBrush AI - Legal Documents

This directory contains all the legal documents for the ToothBrush AI app, ready for deployment on Vercel.

## 📁 Files Included

- `index.html` - Main legal center page with navigation
- `privacy-policy.html` - Comprehensive privacy policy
- `terms-and-conditions.html` - Terms of service and conditions
- `cookie-policy.html` - Cookie and tracking policy
- `vercel.json` - Vercel deployment configuration
- `README.md` - This file

## 🚀 Deployment Instructions

### Option 1: Deploy to Vercel (Recommended)

1. **Install Vercel CLI** (if not already installed):
   ```bash
   npm install -g vercel
   ```

2. **Navigate to the legal directory**:
   ```bash
   cd legal
   ```

3. **Deploy to Vercel**:
   ```bash
   vercel --prod
   ```

4. **Follow the prompts**:
   - Link to existing project or create new one
   - Choose your team/account
   - Confirm deployment

### Option 2: GitHub + Vercel Integration

1. **Create a new GitHub repository** for your legal docs
2. **Upload these files** to the repository
3. **Connect to Vercel**:
   - Go to [vercel.com](https://vercel.com)
   - Import your GitHub repository
   - Deploy automatically

### Option 3: Drag & Drop on Vercel Dashboard

1. **Go to [vercel.com](https://vercel.com)**
2. **Drag the entire `legal` folder** to the deployment area
3. **Deploy instantly**

## 🌐 URL Structure

After deployment, your legal documents will be available at:

- `https://your-domain.vercel.app/` - Legal center homepage
- `https://your-domain.vercel.app/privacy-policy` - Privacy policy
- `https://your-domain.vercel.app/terms-and-conditions` - Terms & conditions
- `https://your-domain.vercel.app/cookie-policy` - Cookie policy

## ✏️ Customization

### Update Contact Information
Replace `andrehabboud1@gmail.com` with your actual contact email in all HTML files.

### Update Dates
Update the "Last Updated" dates in all documents when you make changes.

### Update App Name
If you change your app name from "ToothBrush AI", update it in all HTML files.

### Add Your Logo
Replace the tooth emoji (🦷) with your actual logo by updating the HTML.

## 📱 Mobile App Integration

### Update Your App's Legal URLs
In your React Native app, update the legal URLs to point to your deployed Vercel domain:

```javascript
const LEGAL_URLS = {
  privacyPolicy: 'https://your-domain.vercel.app/privacy-policy',
  termsAndConditions: 'https://your-domain.vercel.app/terms-and-conditions',
  cookiePolicy: 'https://your-domain.vercel.app/cookie-policy',
};
```

### Add Legal Links to Your App
Add legal document links in your app's settings or about screen:

```javascript
// In your SettingsScreen or AboutScreen
<TouchableOpacity onPress={() => Linking.openURL(LEGAL_URLS.privacyPolicy)}>
  <Text>Privacy Policy</Text>
</TouchableOpacity>
```

## 🔒 Security Features

The `vercel.json` file includes security headers:
- Content type protection
- Frame options
- XSS protection

## 📊 Analytics (Optional)

To track visits to your legal pages, you can add analytics:

1. **Google Analytics**:
   ```html
   <!-- Add to <head> section of each HTML file -->
   <script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
   ```

2. **Vercel Analytics**:
   - Enable in your Vercel dashboard
   - No code changes needed

## 🎨 Styling

The legal documents use:
- Modern CSS with gradients
- Responsive design
- Mobile-first approach
- Clean typography
- Consistent branding colors

## 📝 Content Overview

### Privacy Policy Covers:
- Data collection practices
- Health data handling
- Subscription information
- User rights (GDPR, CCPA compliance)
- Third-party services
- Security measures

### Terms & Conditions Cover:
- Service description
- Subscription terms
- User conduct
- Medical disclaimers
- Liability limitations
- Termination policies

### Cookie Policy Covers:
- Cookie types and purposes
- Third-party services
- User choices and controls
- Data retention periods
- Device-specific instructions

## 🆘 Support

If you need help with deployment or customization:
- **Vercel Support**: [vercel.com/docs](https://vercel.com/docs)
- **Contact**: andrehabboud1@gmail.com

---

**Ready to deploy! 🚀**

Your legal documents are now ready for production use with your ToothBrush AI app.
