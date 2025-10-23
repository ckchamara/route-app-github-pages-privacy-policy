# Privacy Policy

**Effective Date:** January 15, 2025

**Last Updated:** October 19, 2025

**App Name:** RouteBus
**Package Names:** com.routebus.app (Production), com.routebus.app.dev (Development)

---

## Introduction

Welcome to RouteBus! We are committed to protecting your privacy and ensuring you have a positive experience while using our application. This Privacy Policy explains how we collect, use, store, and protect your information when you use our bus route management and tracking application.

By using RouteBus, you agree to the collection and use of information in accordance with this policy. If you do not agree with our practices, please do not use the app.

---

## 1. Information We Collect

### 1.1 Information You Provide Directly

**Authentication Information:**
- When you sign in with Google, we collect:
  - Your name
  - Email address
  - Profile picture
  - Google account ID
- This information is used to create and manage your account in Firebase Authentication

**Route Information:**
- Route numbers you create or request
- Starting locations and destination locations
- Route path data including waypoints, stops, and addresses
- Administrative division (province/state) selections
- Route descriptions and notes you add

**Feedback and Contributions:**
- Feedback ratings (thumbs up/down) on routes
- Specific feedback reasons (e.g., "Map is wrong", "Route number is wrong", "Route name is wrong")
- Route edits and improvements you contribute
- Comments or descriptions accompanying your feedback
- Timestamps of when feedback was submitted

**Search and Interaction Data:**
- Search queries for locations and routes
- Places you search for using the autocomplete feature
- Addresses you enter or select

### 1.2 Information Collected Automatically

**Location Data:**
- Your device's GPS coordinates (latitude, longitude) when you use location-based features
- Location accuracy information
- Timestamps of location readings
- Location data is used to:
  - Detect your country and administrative division
  - Center the map on your current location
  - Provide accurate route directions and navigation
  - Show routes relevant to your location
- **Important:** Location tracking only occurs when you actively use the app and have granted location permissions
- We do **NOT** track your location in the background when the app is closed
- You can disable location access at any time in your device settings

**Device and System Information:**
- Device model and manufacturer
- Operating system version and build number
- Device unique identifiers (for analytics purposes only)
- App version number
- Locale and language settings

**Usage and Performance Data:**
- Routes you view and interact with
- Features you use and how frequently
- App performance metrics (load times, crashes)
- Error logs and crash reports
- Session duration and frequency of app usage
- Map interaction data (zoom levels, camera positions)
- Markers and waypoints you place on the map

**Network Information:**
- IP address (for backend API communication)
- Network type (WiFi, mobile data)
- API request/response data

### 1.3 Information from Third-Party Services

**Google Services:**
- Google Maps API provides map data, route directions, and geocoding information
- Google Places API provides location suggestions and address autocomplete
- Google Sign-In provides authentication verification

**Firebase Services:**
- Firebase Authentication provides secure user authentication
- Firebase Crashlytics collects crash reports and error logs
- Firebase Core provides backend infrastructure

---

## 2. How We Use Your Information

We use the collected information for the following purposes:

**To Provide Core Services:**
- Display bus routes and route information on maps
- Allow you to create, edit, and manage routes
- Show routes relevant to your location
- Provide route directions and navigation between waypoints
- Calculate optimal routes using Google Directions API
- Convert addresses to coordinates and vice versa using geocoding

**To Improve User Experience:**
- Remember your preferences (selected country, administrative divisions)
- Provide personalized route recommendations based on your location
- Improve route accuracy based on user feedback
- Optimize app performance and responsiveness
- Enhance map display and navigation features

**To Enable Community Features:**
- Allow users to contribute route improvements and corrections
- Collect and display aggregated route feedback (ratings and statistics)
- Enable route sharing functionality with other users
- Track which routes are most helpful to the community

**For Analytics and Improvements:**
- Understand how users interact with the app
- Identify and fix bugs and crashes
- Improve app features and performance
- Analyze usage patterns to enhance user experience
- Monitor API usage and performance
- Generate analytics reports on route popularity and feedback

**For Security and Compliance:**
- Detect and prevent fraudulent activity
- Enforce our Terms of Service
- Comply with legal obligations and law enforcement requests
- Protect the rights, property, and safety of RouteBus, our users, and the public

---

## 3. Data Storage and Security

**Where Your Data is Stored:**
- **User Authentication:** Firebase Authentication (Google Cloud Infrastructure)
  - Location: Google Cloud data centers (multiple regions)
  - Encrypted at rest and in transit
- **Route Data & Feedback:** MySQL database hosted on Aiven Cloud
  - Location: Aiven Cloud infrastructure
  - Encrypted database connections
- **Map Images:** Cloudflare R2 object storage
  - Location: Cloudflare global network
  - Encrypted storage
- **Local Device Storage:** Your device's secure local storage
  - Preferences and cached data
  - Encrypted using device-level encryption

**How We Protect Your Data:**
- All data transmission uses HTTPS/TLS encryption (minimum TLS 1.2)
- Database access is restricted with strong authentication and password protection
- We implement industry-standard security measures to protect against unauthorized access
- Regular security updates and patches
- Access controls limit who can view sensitive data
- Sensitive credentials are stored securely and never logged

**Data Retention:**
- **Account Data:** Retained as long as your account is active
  - Deleted upon account deletion request (within 30 days)
- **Route Data:** Retained indefinitely to maintain service quality and community contributions
  - Can be deleted by the route creator
  - Anonymized if account is deleted
- **Feedback Data:** Retained for analytics and improvement purposes
  - Aggregated and anonymized for reporting
  - Individual feedback can be deleted upon request
- **Crash Reports:** Retained for 90 days for debugging purposes
  - Automatically purged after retention period
- **Location Data:** Not permanently stored
  - Used only for current session
  - Not retained after app closes

---

## 4. Third-Party Services and Data Sharing

We use the following third-party services that may collect and process your information:

### 4.1 Google Services

**Google Maps Platform:**
- **Google Maps API:** For displaying interactive maps, route visualization, and map controls
- **Google Directions API:** For calculating optimal routes between waypoints
- **Google Geocoding API:** For converting addresses to coordinates and vice versa
- **Google Places API:** For location autocomplete, address search, and place suggestions
- **Google Sign-In:** For secure authentication with your Google account
- **Data Shared:** Location coordinates, addresses, route waypoints, search queries
- **Privacy Policy:** https://policies.google.com/privacy
- **Terms of Service:** https://cloud.google.com/maps-platform/terms

### 4.2 Firebase Services (Google Cloud)

**Firebase Authentication:**
- Secure user authentication and session management
- Data Shared: Email, name, profile picture, authentication tokens
- Privacy Policy: https://firebase.google.com/support/privacy

**Firebase Crashlytics:**
- Crash reporting and error tracking
- Data Shared: Crash logs, stack traces, device information, app version
- Used only in production builds (disabled in debug builds)
- Privacy Policy: https://firebase.google.com/support/privacy

**Firebase Core:**
- Backend infrastructure and data synchronization
- Privacy Policy: https://firebase.google.com/support/privacy

### 4.3 Cloud Infrastructure Providers

**Aiven Cloud (MySQL Database):**
- Hosts our route data, user feedback, and analytics database
- Data Shared: All route information, feedback, user contributions
- Privacy Policy: https://aiven.io/privacy
- Data Processing Agreement: Available upon request

**Cloudflare R2 (Object Storage):**
- Stores generated map images and route visualizations
- Data Shared: Map images, route paths
- Privacy Policy: https://www.cloudflare.com/privacypolicy/
- Data Processing Agreement: Available upon request

### 4.4 Important Notes About Third-Party Services

- Each third-party service has its own privacy policy and data handling practices
- We encourage you to review their privacy policies to understand how they handle your data
- We are not responsible for third-party privacy practices
- We have Data Processing Agreements with all infrastructure providers
- All third-party services comply with GDPR and international data protection standards

---

## 5. Data Sharing and Disclosure

**We Do Not Sell Your Data:**
- We will **never** sell, rent, lease, or trade your personal information to third parties
- We do not share your data with advertisers or marketing companies
- We do not use your data for targeted advertising

**When We May Share Data:**

**With Your Explicit Consent:**
- When you explicitly agree to share information
- When you choose to share a route with other users
- When you submit feedback or bug reports

**With Service Providers:**
- With trusted third-party services (listed above) necessary to operate the app
- Only the minimum data necessary to provide the service
- Under strict confidentiality agreements

**For Legal Compliance:**
- If required by law, court order, or government regulation
- To comply with legal obligations
- To respond to lawful requests from authorities
- We will notify you of such requests when legally permitted

**For Safety and Security:**
- To protect the rights, property, or safety of RouteBus, our users, or the public
- To detect, prevent, or address fraud, security, or technical issues
- To enforce our Terms of Service and other agreements

**In Case of Business Transfer:**
- If RouteBus is acquired, merged, or sold, your data may be transferred as part of that transaction
- We will notify you of any such change and any choices you may have

**Public Information:**
- Routes you create are visible to other users of the app
- Route feedback (ratings) is aggregated and displayed publicly
- Your name may be associated with routes you create
- You can control the visibility of your routes through app settings
- Aggregated and anonymized analytics may be published

---

## 6. Your Rights and Choices

You have the following rights regarding your data:

**Access Your Data:**
- View your account information in Settings > Account Details
- Request a copy of all your personal data by contacting us
- We will provide your data in a portable format within 30 days

**Update Your Data:**
- Edit your account information in Settings > Account Details
- Update your profile picture and name
- Modify your route information and contributions

**Delete Your Data:**
- Delete individual routes you have created
- Delete your account and associated personal data
- Account deletion will remove your personal information within 30 days
- Public contributions (routes, feedback) may be retained in anonymized form for community benefit

**Control Location Access:**
- Enable or disable location access in your device settings
- The app will still function with limited features if location is disabled
- You can revoke location permissions at any time

**Opt-Out of Data Collection:**
- Disable crash reporting in app settings (if available)
- Stop using the app at any time
- Uninstalling the app will stop all data collection

**Data Portability:**
- Request your data in a standard, portable format
- Transfer your data to another service
- Contact us for assistance with data portability

**Right to Withdraw Consent:**
- Withdraw consent for data processing at any time
- This will not affect the legality of processing before withdrawal

**Right to Object:**
- Object to certain types of data processing
- Request restriction of data processing
- Contact us to exercise these rights

---

## 7. Children's Privacy

**Age Restriction:**
- RouteBus is not intended for children under the age of 13
- We do not knowingly collect personal information from children under 13
- We do not knowingly allow children under 13 to create accounts or use the app

**Parental Responsibility:**
- Parents and guardians are responsible for monitoring their children's use of the app
- If you are a parent or guardian and believe your child has provided us with personal information, please contact us immediately
- We will delete such information within 30 days of verification

**COPPA Compliance:**
- We comply with the Children's Online Privacy Protection Act (COPPA)
- We do not collect more information from children than necessary
- We do not use children's information for marketing or advertising purposes

---

## 8. Privacy Compliance and Legal Basis

**GDPR Compliance (European Users):**
- We comply with the General Data Protection Regulation (GDPR)
- Legal basis for processing:
  - **Consent:** For authentication and optional features
  - **Contract:** To provide the app services
  - **Legitimate Interest:** For analytics and security
  - **Legal Obligation:** To comply with laws and regulations
- You have rights under GDPR including access, rectification, erasure, and portability
- Data transfers outside the EU are protected by appropriate safeguards

**CCPA Compliance (California Users):**
- We comply with the California Consumer Privacy Act (CCPA)
- You have the right to:
  - Know what personal information is collected
  - Delete personal information collected from you
  - Opt-out of the sale of your personal information (we do not sell data)
  - Non-discrimination for exercising your CCPA rights

**Other Privacy Laws:**
- We comply with applicable privacy laws in all jurisdictions where we operate
- This includes laws in Sri Lanka, India, and other countries

**Data Protection Officer:**
- For privacy inquiries, contact: privacy@routebus.app
- We will respond to all privacy requests within 30 days

---

## 9. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect:
- Changes in our data practices
- New features or services
- Legal, operational, or regulatory requirements
- Feedback from users

**How We Notify You:**
- We will post the updated policy in the app
- The "Last Updated" date at the top will be changed
- For significant changes, we will notify you via:
  - In-app notification
  - Email notification (if we have your email)
  - Prominent notice in the app

**Your Rights Upon Changes:**
- You will have the opportunity to review changes before they take effect
- For material changes, we will request your consent
- Continued use of the app after changes constitutes acceptance of the updated policy
- You can delete your account if you disagree with changes

**Archive of Previous Versions:**
- Previous versions of this policy are available upon request
- Contact us to request a specific version

---

## 10. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy or your data, please contact us:

**Email:** privacy@routebus.app
**Support Email:** support@routebus.app
**In-App:** Settings > Account Details > Contact Support

**Data Subject Requests:**
- For access, deletion, or portability requests, email: privacy@routebus.app
- Include "Data Subject Request" in the subject line
- Provide your account email and specific request details

**Response Time:**
- We will respond to your inquiry within 30 days
- For complex requests, we may need additional time (up to 90 days)
- We will notify you if we need more time

**Escalation:**
- If you are not satisfied with our response, you have the right to lodge a complaint with your local data protection authority

---

## 11. International Data Transfers

**Data Location:**
- Your data is stored in multiple geographic locations:
  - Google Cloud (Firebase) - Multiple regions
  - Aiven Cloud - EU and US regions
  - Cloudflare - Global CDN

**Data Protection:**
- All international transfers are protected by:
  - Standard Contractual Clauses (SCCs)
  - Data Processing Agreements (DPAs)
  - Appropriate safeguards under GDPR

**Your Rights:**
- You have the right to know where your data is stored
- You can request information about data transfer mechanisms
- Contact us for details about specific data locations

---

## 12. Security Incident Notification

**In Case of a Data Breach:**
- We will notify affected users without undue delay
- Notification will include:
  - Description of the incident
  - Types of data affected
  - Likely consequences
  - Measures taken to address the breach
  - Contact information for further inquiries
- We will notify relevant authorities as required by law

**Your Responsibilities:**
- Keep your password secure
- Do not share your login credentials
- Report suspicious activity immediately
- Keep your device software updated

---

## 13. Your Consent

By using RouteBus, you:
- Consent to this Privacy Policy and agree to its terms
- Acknowledge that you have read and understood this policy
- Agree to the collection and use of information as described
- Understand that you can withdraw consent at any time

**Withdrawal of Consent:**
- You can withdraw consent by deleting your account
- You can disable specific features (like location access) in settings
- Withdrawal will not affect the legality of processing before withdrawal

---

## 14. Additional Information

**Cookies and Tracking:**
- RouteBus does not use cookies or tracking pixels
- We use local device storage for preferences only
- Third-party services (Google, Firebase) may use their own tracking mechanisms

**Third-Party Links:**
- The app may contain links to third-party websites and services
- We are not responsible for their privacy practices
- Review their privacy policies before providing information

**App Permissions:**
- RouteBus requests the following permissions:
  - **Location:** For GPS-based features
  - **Internet:** For API communication
  - **Camera:** For future features (if applicable)
  - **Storage:** For caching and local data
- You can revoke permissions at any time in device settings

**Accessibility:**
- This privacy policy is available in multiple formats
- Contact us if you need an accessible version

---

**Thank you for trusting RouteBus with your information. We are committed to protecting your privacy and providing you with the best possible experience.**

**Last Updated:** October 19, 2025
**Version:** 2.0

