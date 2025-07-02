# ETCP-Website-Prototype

### **Technical and Functional Documentation: Eco-Tourism Cloud Platform (ETCP) Website Prototype**
#### **Document Version:** 1.0
#### **Date:** July 2, 2025
#### **Prepared For:** ETCP Board of Directors / Academic Evaluation
#### **Purpose:** This document provides a comprehensive technical and functional overview of the Eco-Tourism Cloud Platform (ETCP) website prototype. It details the implemented user interface (UI) and user experience (UX) elements, aligns them with the strategic vision outlined in the project brief, and identifies areas for future development towards a fully functional platform.

### 1. Project Overview: Eco-Tourism Cloud Platform (ETCP)
   
The Eco-Tourism Cloud Platform (ETCP) is an innovative cloud-based solution designed to revolutionize how eco-conscious travelers discover, plan, and engage with sustainable tourism experiences globally. Developed by a visionary Sri Lankan start-up, ETCP aims to foster a deeper connection between users and the natural world, promoting eco-friendly practices and supporting local communities.

**1.1 Key Features (from Project Brief)**

**The ETCP vision encompasses several core features:**

Eco-Explorer Network (EEN): A community-driven platform for eco-tourism providers to register, publish offerings, manage bookings, view analytics, handle payments, showcase sustainability, and receive feedback.

Eco-Discovery Hub: A dynamic search and discovery tool for eco-tourism experiences based on location, activity type, sustainability rating, and other filters. It aims to facilitate booking, eco-pass subscriptions, and access to detailed experience information.

Eco-Journeys: A personalized dashboard for users to manage bookings, subscriptions, and favorite experiences, offering viewing/sorting options, a wishlist, and "Discover Similar" recommendations.

ETCP Voyager: An interactive map and planner for crafting eco-tourism itineraries, integrating visual map interfaces, route planning tools, sustainability impact estimation, and seamless addition of experiences from the Eco-Discovery Hub.

Settings & Personalization: Features allowing users to customize their ETCP experience, including visual themes, language preferences, accessibility options, and payment/subscription management.

### 2. Website Architecture & Technologies

The current ETCP website is implemented as a static frontend prototype, primarily focusing on demonstrating the user interface and user experience flows. It does not include backend logic, database integration, or live API calls.

**2.1 Core Technologies**

HTML5: Provides the semantic structure and content of all web pages.

CSS3: Used for styling, layout, and visual presentation. All custom CSS is embedded directly within <style> tags in each HTML file, alongside Bootstrap's framework.

JavaScript (Vanilla JS): Handles client-side interactivity, UI animations, form validation, and content switching. All custom JavaScript is embedded directly within <script> tags in each HTML file.

Bootstrap 5.3.3: A robust, mobile-first CSS framework used for responsive grid layouts, navigation components (navbar, togglers), form styling, and various utility classes, ensuring cross-device compatibility.

Font Awesome 6.4.0: Provides scalable vector icons used throughout the site for navigation, social media, form elements, and dashboard features.

Google Fonts (Poppins): Ensures consistent and modern typography across the platform.

**2.2 Design Principles**

The prototype adheres to several key design principles:

Responsiveness: Utilizes Bootstrap's grid system and custom media queries to ensure optimal viewing and interaction across desktop, tablet, and mobile devices.

Visual Consistency: A consistent color palette (predominantly greens), typography (Poppins font), and design elements (rounded corners, subtle shadows) are maintained across all pages, reinforcing brand identity.

Intuitive Navigation: A fixed top navigation bar with clear links facilitates easy movement between main sections.

Engaging Interactivity: Subtle CSS animations (fade-in, slide-in) triggered by JavaScript's Intersection Observer enhance user engagement without being distracting.

### 3. Detailed Page Analysis

This section provides a detailed breakdown of each page within the ETCP website prototype, highlighting its purpose, implemented UI/UX elements, and alignment with the project brief.

**3.1 Home Page (index.html)**

Purpose: To serve as the primary entry point to the ETCP platform, introducing its mission, showcasing trending destinations, and guiding users towards key functionalities like property registration and trip planning.

**Key UI Components & Layout:**

Fixed Navbar: Consistent across the site, offering navigation to core pages and a language/sign-in option.

Hero Carousel: A full-width, image-based slider that visually introduces the platform's theme.

Welcome Section: Textual introduction to ETCP's vision and Sri Lankan origin, paired with a large illustrative image.

Trending Destinations Grid: A visually appealing CSS Grid layout showcasing popular eco-tourism locations with images and names. Includes an "Explore More" card.

Register Banner: A prominent, animated call-to-action for property providers.

Rewards Box: Encourages user sign-in for benefits.

Footer: Comprehensive site map, social media links, and copyright information.

**Core Functionality (as implemented in prototype):**

Navigation: Links to register.html, plan.html, about.html, and signin.html.

Navbar Shrink: The navigation bar visually shrinks on scroll.

Scroll Animations: Elements like the welcome text, destination cards, and banners fade and slide into view as the user scrolls.

Call-to-Action: Clickable areas for "Explore More" (to plan.html), "Register" (to register.html), and "Sign in" (to signin.html).

**Styling Highlights:**

Extensive use of --primary-green and linear-gradient backgrounds.

Custom nav-link::after for hover underline effect.

animate-on-scroll classes with data-anim attributes for directional animations.

dest-grid uses display: grid for a responsive and visually engaging destination layout.

blink-1, blink-2, and chase animations for the "Register Banner."

**Scenario Alignment & Future Scope:**

Alignment: This page effectively introduces the ETCP concept and visually aligns with the eco-tourism theme. It serves as a good entry point to the "Eco-Discovery Hub" (plan.html) and "Eco-Explorer Network" (register.html).

Future Enhancements: In a full system, the "Trending Destinations" would be dynamically populated from a database, potentially personalized. The "Rewards" section would integrate with a real user account system.

Home Page - Full View

Figma design

![Home](https://github.com/user-attachments/assets/0ad61727-aec2-4d51-9cbe-14f7552e7382)

Web design

![_C__Users_Devindu%20Malshan_Desktop_HND_UEID_Assignment_ETCP%20Design_ETCP%20Website%20Prototype_index html](https://github.com/user-attachments/assets/94d658ce-be1b-44e8-be49-e202bd026c26)

Home Page - Trending Destinations Grid

![Screenshot 2025-07-02 120733](https://github.com/user-attachments/assets/c047b037-fb30-4293-a0f2-ea136c4cb9ca)

Home Page - Register Banner

![Screenshot 2025-07-02 120834](https://github.com/user-attachments/assets/c0e14a62-cf3e-4808-8dcc-bb741eeb9e7e)

**3.2 Plan Your Trip Page (plan.html - Eco-Discovery Hub)**

Purpose: To enable users to search, filter, and discover eco-tourism experiences based on various criteria, serving as the primary interface for the "Eco-Discovery Hub."

**Key UI Components & Layout:**

Main Search Pill: A prominent, sticky search bar at the top with fields for location, dates, and guests.

Filter Sidebar: A collapsible left-hand sidebar containing extensive filtering options (Budget, Meals, Property type, Activity, Rating, Facilities, Policy, Group).

Results Area: Displays property listings, with options to switch between List and Grid views.

Property Cards: Individual listings showing images, names, locations, prices, ratings, and deal badges.

Recommendations & Offers: Sections for suggested destinations and promotions.

"Show on Map" Section: A placeholder for the "ETCP Voyager" feature.

**Core Functionality (as implemented in prototype):**

Client-Side Filtering: All filters (location, budget range slider, checkboxes, radio buttons) dynamically filter a static allProperties JavaScript array.

Guest Selector: Interactive increment/decrement for adults and children.

Budget Slider: Custom dual-thumb range slider with visual fill.

View Toggle: Switches between a list-view (flexbox) and grid-view (CSS Grid) for property display.

Sorting: Sorts properties by Price or Rating (client-side).

Wishlist Button: Adds/removes property IDs to/from a client-side wishlistItems array (not persistent).

Dynamic Content Insertion: Inserts static "Offers" and "Ad" cards at specific intervals within the property listings.

**Styling Highlights:**

Customized Bootstrap form controls and input fields.

Extensive use of display: flex and display: grid for responsive layouts.

Custom checkbox and radio button styling.

Animations for guest popover (fadeInScale) and filter section headers.

Distinctive styling for result-card, recommendation-card, and offer-card.

Detailed media queries for mobile responsiveness, especially for the search pill and result card layouts.

**Scenario Alignment & Future Scope:**

Alignment: This page is a strong visual and interactive prototype for the "Eco-Discovery Hub," demonstrating comprehensive filtering capabilities.

**Future Enhancements:**

Backend Integration: Property data (allProperties) would be fetched from a database via an API.

Real Booking Flow: "See availability" would lead to a functional booking process, integrating with dates and payment.

Persistent Wishlist: Wishlist items would be stored in a user's profile on the backend.

ETCP Voyager Integration: The "Show on map" would become a fully interactive map with live property data and route planning.

Detailed Experience Pages: Clicking on a property card would lead to a dedicated page with more information, including sustainability practices and reviews.

[Screenshot: Plan Your Trip - Main Search & Filters]

[Screenshot: Plan Your Trip - Property Listings (Grid View)]

[Screenshot: Plan Your Trip - Property Listings (List View)]

3.3 Register Your Property Page (register.html - Eco-Explorer Network)

Purpose: To provide a clear and intuitive interface for eco-tourism providers to register their properties with the ETCP platform, forming the entry point for the "Eco-Explorer Network."

**Key UI Components & Layout:**

Welcome Section: Introduces ETCP to providers, highlighting benefits, paired with a large image.

Registration Form: A multi-field form for collecting property name, address, contact details, and email.

Media Upload Sections: Dedicated areas for uploading property photos and videos, with placeholder icons.

Register Button: A prominent call-to-action to submit the form.

**Core Functionality (as implemented in prototype):**

Form Input: Standard HTML text, tel, and email input fields.

Basic Client-Side Validation: Uses HTML5 required attribute and Bootstrap's was-validated class for visual feedback on form submission.

Simulated Submission: On submission, logs data to the console and displays a simple alert() message (placeholder for backend interaction).

File Upload Placeholders: input type="file" elements are present, but the actual file handling and storage are not implemented.

Scroll Animations: Sections and elements fade and slide into view.

**Styling Highlights:**

Gradient background for the welcome section.

Custom green borders and rounded corners for form controls.

Dashed-border upload-box elements with centered Font Awesome icons for visual appeal.

Responsive layout for form fields and upload sections.

Scenario Alignment & Future Scope:

Alignment: This page successfully prototypes the initial "register" aspect of the "Eco-Explorer Network."

**Future Enhancements:**

Backend Integration: Form data and uploaded files would be sent to a server-side API for processing and storage in a database.

Advanced Validation: More robust client-side and server-side validation.

User Authentication: Integration with a provider authentication system.

Provider Dashboard: After registration, providers would access a dedicated dashboard for managing listings, bookings, analytics, and payments, as outlined in the brief.

Sustainability Details: Fields for sustainability certifications and practices would be added.

[Screenshot: Register Your Property - Full View]

[Screenshot: Register Your Property - Registration Form Fields]

[Screenshot: Register Your Property - Upload Sections]

**3.4 About Us Page (about.html)**

Purpose: To inform users about ETCP's mission, values, unique selling propositions, and commitment to sustainability and local communities.

**Key UI Components & Layout:**

Standard Navbar & Footer: Consistent with other pages.

Content Sections: Divided into distinct sections: "About Us," "Our Mission," "What Sets Us Apart," "Our Team," "Supporting Local Communities," and "Join Us."

Alternating Image/Text Layout: Uses Bootstrap's grid system to alternate image and text column positions for visual variety.

List of Unique Features: "What Sets Us Apart" section uses an unordered list to highlight key differentiators.

Team Banner Image: A wide image representing the ETCP team.

**Core Functionality (as implemented in prototype):**

Navigation: Standard links to other pages.

Navbar Shrink: The navigation bar visually shrinks on scroll.

Scroll Animations: All content sections and list items fade and slide into view.

**Styling Highlights:**

Consistent section-heading and section-text styles.

Alternating background colors (#f9f9f9) for sections to improve readability and visual separation.

Rounded images (img-fluid rounded).

Slightly slower transition for animate-on-scroll for a more deliberate reveal.

**Scenario Alignment & Future Scope:**

Alignment: This page effectively communicates the brand's story and values, aligning with the brief's emphasis on eco-consciousness and community support.

Future Enhancements: Content could be managed via a CMS. Could include dynamic elements like testimonials or team member profiles.

[Screenshot: About Us - Full View]

[Screenshot: About Us - Our Mission Section]

**3.5 Sign In Page (signin.html)**

Purpose: To provide a user-friendly interface for existing users to sign in to their ETCP accounts, serving as the gateway to "Eco-Journeys."

**Key UI Components & Layout:**

Centralized Sign-in Card: A prominent, visually appealing card positioned centrally on the page.

Email Input Form: A single field for email entry, with a "Continue with email" button.

Message Display Area: A dynamic area for displaying success or error messages.

Divider: "or use one of these options" separator.

Social Login Buttons: Placeholder icons for Google, Apple, and Facebook sign-in.

Terms & Privacy Links: Legal disclaimers.

Copyright Information: Footer text within the card.

**Core Functionality (as implemented in prototype):**

Navbar Shrink: Consistent with other pages.

Email Input Validation: Uses HTML5 type="email" and required for basic browser validation.

Button Enable/Disable: The "Continue with email" button is disabled until a valid email format is entered.

**Simulated Authentication:**

Compares the entered email against a hardcoded correctEmail (brooke.higgins25@etcp.com).

Displays success/error messages (showMessage function) dynamically.

Upon "successful" match, simulates a redirect to dashboard.html after a short delay.

Animations: The sign-card itself fades and slides down on page load. Messages also animate in/out.

**Styling Highlights:**

Gradient background for the signin-section.

sign-card with box-shadow and fadeInDown animation.

Custom green borders and rounded corners for inputs and buttons.

Styling for the divider-with-text and circular social-btn elements.

Distinctive feedback-message styles for success and error states.

**Scenario Alignment & Future Scope:**

Alignment: This page provides a clear UI for user sign-in, aligning with the need for user accounts to access personalized features.

**Future Enhancements:**

Real Backend Authentication: Integrate with a robust authentication system (e.g., Firebase Auth, OAuth providers) for secure user login and session management.

Password Field: Implement a password input and corresponding "Forgot Password" functionality.

Account Creation: Provide a clear path for new users to register an account (e.g., a "Sign Up" link or integrated flow).

Social Login Integration: Make Google, Apple, and Facebook login buttons fully functional.

Error Handling: More specific error messages from the backend (e.g., "User not found," "Incorrect password").

[Screenshot: Sign In Page - Full View]

[Screenshot: Sign In Page - Email Input & Buttons]

**3.6 Dashboard Page (dashboard.html - Eco-Journeys)**

Purpose: To serve as the personalized user dashboard, allowing users to manage their bookings, subscriptions, and access other account-related features, forming the core of "Eco-Journeys."

**Key UI Components & Layout:**

Welcome Modal: A temporary, animated overlay greeting the user on dashboard entry.

Two-Column Layout: A fixed-width left sidebar (dashboard-sidebar) and a dynamic main content area (dashboard-content).

User Profile: Displays a placeholder profile picture and user name in the sidebar.

Sidebar Menu: Navigation links to various dashboard sections (My bookings, Notification, Wishlist, Subscriptions, Sustainability impact, Settings, Feedback, Help).

Content Sections: Each sidebar link corresponds to a distinct content section, displayed dynamically.

My Bookings Table: Displays a list of static example bookings with details and action buttons.

Recommendations Grid: A grid of static destination recommendations.

Offers Card: A prominent card promoting special deals.

Placeholder Sections: notification, wishlist, subscriptions, sustainability, settings, feedback, and help sections are present with static content or basic UI elements.

**Core Functionality (as implemented in prototype):**

Welcome Modal Animation: Displays an animated "Welcome traveler!" modal on page load, then fades out to reveal the dashboard.

Navbar Shrink: Consistent with other pages.

Sidebar Navigation: Clicking sidebar links dynamically switches the visible content section in the main area using JavaScript, with fade-in/slide-up transitions.

Initial Active Section: "My bookings" is set as the default active section.

Static Data: All booking, recommendation, and offer data is hardcoded.

Placeholder Interactions: Subscription toggles are present but do not persist state. Action buttons in tables and forms are non-functional placeholders.

**Styling Highlights:**

Light green background for the dashboard-container and sidebar-bg.

welcome-modal-content with gradient and bounce animation.

user-profile with fadeInScale and fadeInUp animations.

sidebar-menu li a with a sophisticated sliding green background on hover using a ::before pseudo-element.

Distinctive active state for sidebar links (left border, background color).

content-section animations (opacity, transform) for smooth transitions.

Custom table styling with rounded rows and spacing.

recommendation-card and offer-card with box-shadow and hover effects.

Extensive media queries to transform the two-column layout into a stacked, horizontally-scrolling mobile layout for the sidebar.

**Scenario Alignment & Future Scope:**

Alignment: This page provides a strong visual and interactive framework for "Eco-Journeys," demonstrating the personalized dashboard concept. The presence of sections like "Wishlist," "Subscriptions," and "Sustainability impact" directly aligns with the brief.

**Future Enhancements:**

Backend Integration: All content (user profile, bookings, notifications, wishlist, subscriptions, sustainability data) would be fetched dynamically from a backend database via APIs.

Functional Actions: "View" and "Cancel" booking buttons would trigger real actions. Subscription toggles would update user preferences. Feedback forms would submit data.

Dynamic Recommendations: The "Recommendations" would be powered by a recommendation engine.

Real-time Notifications: Integration with a real-time notification system.

ETCP Voyager Integration: The "Sustainability impact" section would integrate with the ETCP Voyager's estimates.

User Management: Full profile editing, password changes, and account linking in "Settings."

[Screenshot: Dashboard - Full Desktop View]

[Screenshot: Dashboard - User Profile & Sidebar Menu]

[Screenshot: Dashboard - My Bookings Table]

[Screenshot: Dashboard - Recommendations & Offers]

[Screenshot: Dashboard - Mobile View (Sidebar collapsed/scrolling)]

### 4. Cross-Cutting Concerns

**4.1 Responsiveness**

The entire website prototype is built with a mobile-first approach, leveraging Bootstrap's responsive grid system and extensive custom media queries. This ensures that the layout, typography, and interactive elements adapt seamlessly across various screen sizes, from mobile phones to large desktop displays. Specific adjustments are evident in the main search bar on plan.html, the dashboard's sidebar, and general element stacking.

**4.2 Accessibility**

Basic accessibility considerations have been integrated:

Semantic HTML5: Use of elements like nav, main, section, form, label, table, thead, tbody, th improves document structure and readability for assistive technologies.

alt Attributes: All <img> tags include descriptive alt attributes.

aria- Attributes: Bootstrap components (e.g., navbar-toggler) incorporate aria-controls, aria-expanded, and aria-label. Social media links also use aria-label.

Form Labels: All input fields are correctly associated with <label> elements using for and id.

Keyboard Navigation: Standard HTML elements and Bootstrap components provide inherent keyboard focus and interaction. Custom focus styles on form inputs enhance visibility for keyboard users.

**4.3 Frontend Performance**

CDN Usage: External libraries (Bootstrap, Font Awesome, Google Fonts) are loaded from Content Delivery Networks (CDNs), leveraging browser caching and distributed servers for faster delivery.

JavaScript Placement: All custom JavaScript is placed at the end of the <body> tag, preventing render-blocking and allowing the HTML content to load and display before scripts execute.

Intersection Observer: Used for scroll-triggered animations, which is more performant than traditional scroll event listeners as it avoids continuous calculations.

Inline CSS/JS: While convenient for prototyping, for a production site, external CSS/JS files would be preferred for better caching and modularity.

Image Optimization: While not directly controllable within the HTML, the choice of image formats and compression would be a critical performance consideration for a live site.

**4.4 Branding & Visual Consistency**

The prototype effectively establishes a consistent brand identity:

Color Palette: A cohesive green-based color scheme (--primary-green, --hover-green, various light green tints) is used throughout, reinforcing the "eco" theme.

Typography: The "Poppins" font family is consistently applied, contributing to a modern and clean aesthetic.

Design Elements: Rounded corners on cards, buttons, and input fields, along with subtle box-shadow effects, create a soft, inviting, and contemporary feel.

Iconography: Font Awesome icons are used consistently to enhance visual communication and user guidance.

### 5. Prototype Limitations & Future Enhancements
   
The current ETCP website is a User Interface and User Experience prototype, designed to visualize the platform's concept, test design choices, and gather feedback on usability. As such, it has inherent limitations as a fully functional web application.

**5.1 Key Backend Dependencies & Missing Functionalities**

The following core features, outlined in the project brief, are not implemented in this frontend prototype and represent significant backend development requirements:

User Authentication & Authorization: Real user sign-in, account creation, password management, and secure session handling.

Database Integration: No persistent storage for user profiles, property listings, bookings, wishlists, subscriptions, or analytics data. All dynamic data is currently static or client-side ephemeral.

API Development: No backend APIs to handle data retrieval, form submissions, booking requests, payment processing, or real-time updates.

Booking System: The complete booking flow (availability checks, reservation, confirmation, payment processing) is not functional.

Payment Gateway Integration: No integration with payment providers for transactions.

Dynamic Content Management: Property listings, recommendations, offers, and potentially "About Us" content are static; a Content Management System (CMS) would be needed for dynamic updates.

Analytics & Reporting: Provider analytics and user sustainability impact tracking are conceptual placeholders.

Interactive Mapping (ETCP Voyager): The map feature is static; a fully interactive map with real-time data overlays, route planning, and impact estimation requires significant mapping API integration (e.g., Google Maps API, Mapbox).

Recommendation Engine: The "Discover Similar" and "Recommendations" features lack the backend logic to provide personalized, data-driven suggestions.

Notification System: Real-time or push notifications are not implemented.

**5.2 Areas for Future UI/UX Iteration (Based on Assignment Context)**

Beyond backend integration, the prototype serves as a foundation for further UI/UX refinement, as per the assignment's iterative design methodology:

Streamlining Booking Process: Once backend is integrated, focus on optimizing the user flow from discovery to confirmed booking.

Enriching Eco-Education Content: Integrate more detailed information on sustainability practices within property listings and the "Sustainability Impact" section.

Personalization: Develop UI elements for customizing themes, language, and accessibility settings, and ensure these preferences are saved.

Feedback Integration: Implement the feedback form to capture user input and integrate it into a review process.

Error & Loading States: Design and implement clear UI feedback for network errors, loading times, and form submission statuses.

### 6. Conclusion

The ETCP website prototype effectively demonstrates the envisioned user interface and experience for an eco-tourism platform. It showcases a clean, responsive design and intuitive navigation, providing a strong visual foundation for the "Eco-Discovery Hub," "Eco-Journeys," and the "Eco-Explorer Network" registration.

While the current implementation is frontend-focused, it serves as an invaluable tool for conducting usability testing and gathering critical user feedback on the design and interaction flows. The identified future enhancements highlight the necessary steps to evolve this prototype into a fully functional, robust, and impactful Eco-Tourism Cloud Platform, aligning with the company's corporate goal of connecting eco-conscious travelers with sustainable experiences worldwide.
