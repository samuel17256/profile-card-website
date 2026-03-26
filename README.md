# Profile Card Website

A responsive team profile card website showcasing team members with elegant hover effects and social media links.

## Features

- **Responsive Design**: Works seamlessly across desktop, tablet, and mobile devices
- **Interactive Cards**: Hover effects with animated profile pictures and social media icons
- **Modern UI**: Clean, professional design with custom fonts and styling
- **Team Showcase**: Display team member information including names, roles, and descriptions
- **Individual Profile Pages**: Click on any team member card to view their detailed profile page
- **Detailed Profiles**: Each team member has a dedicated page with biography, skills, and contact information

## Technologies Used

- **HTML5**: Semantic markup for structure
- **Tailwind CSS v4**: Utility-first CSS framework for styling
- **Custom CSS**: Additional animations and effects
- **Google Fonts**: Typography with Josefin Sans and Barlow Semi Condensed
- **Font Awesome**: Social media icons

## Project Structure

```
profile-card-website/
├── index.html          # Main team overview page
├── timothy.html        # Dev Timothy's profile page
├── eazee.html          # Dev Eazee's profile page
├── nanbam.html         # Dev Nanbam's profile page
├── magwah.html         # Dev Magwah's profile page
├── mabas.html          # Dev Mabas's profile page
├── package.json        # Project dependencies
├── README.md          # This file
└── src/
    ├── style.css      # Custom styles and Tailwind imports
    └── output.css     # Compiled Tailwind CSS
```

## Setup and Installation

1. **Clone or download the project**

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Build the CSS:**
   ```bash
   npx @tailwindcss/cli -i ./src/style.css -o ./src/output.css --watch
   ```
   Or for production:
   ```bash
   npx @tailwindcss/cli -i ./src/style.css -o ./src/output.css
   ```

4. **Open the website:**
   Open `index.html` in your web browser or serve it with a local server.

## Usage

Simply open the `index.html` file in any modern web browser or serve it with a local server. The website displays team profile cards with:

- Profile pictures
- Names and job titles
- Brief descriptions
- Social media links (Facebook, Twitter, Google+, LinkedIn)

### Interacting with Profile Cards

**Hover Effects**: Hover over the cards to see the interactive animation effects - the profile picture shrinks and expands within a circle, revealing social media icons.

**Clicking on Cards**: Click on any team member's card to navigate to their detailed profile page. Each profile page includes:
- Full-size profile picture with gradient header
- Detailed biography and professional background
- Skills and expertise section with key technologies
- Quick contact links to social media profiles
- Navigation button to return to the team overview

### Returning to Team Overview

From any individual profile page, click the "Back to Team" button in the navigation bar to return to the main index page.

## Customization

### Adding Team Members

To add more team members:

1. **Update the main page (`index.html`)**: Duplicate a card structure and update:
   - Profile image URL
   - Name (`h3` tag)
   - Job title (`h4` tag)
   - Description (`p` tag)
   - Social media links (`href` attributes)

2. **Create a new profile page**: Create a new HTML file (e.g., `newmember.html`) based on the existing profile pages and update:
   - Title tag with the member's name
   - Profile image URL
   - Member name and job title
   - Biography and background information
   - Skills section with relevant technologies
   - Social media links

3. **Link the card to the profile page**: Update the main card's anchor tag to point to the new profile page:
   ```html
   <a href="newmember.html">
     <!-- card content -->
   </a>
   ```

### Styling Changes

Modify `src/style.css` for custom styles. The file imports Tailwind CSS and includes custom animations for the hover effects.

### Fonts

The website uses Google Fonts. To change fonts, update the Google Fonts link in the HTML files and the `font-family` in `src/style.css`.

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Contributing

Feel free to submit issues and enhancement requests!
