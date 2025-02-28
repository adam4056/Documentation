---
layout: default
---

# Documentation

This documentation will guide you through customizing the provided template. The template consists of two main files: `index.html` and `styles.css`.

## index.html

This file contains the structure of your webpage. Here are the key sections you might want to customize:

1. **Title and Favicon**

    The title and favicon are displayed in the browser tab. You can change the title to your name or nickname and update the favicon to your preferred icon.

    ```html
    <title>David Smith</title> <!-- your name or nickname -->
    <link rel="icon" href="favicon.png" type="image/x-icon"> <!-- favicon -->
    ```

2. **Profile Section**

    This section contains your profile photo and name. You can replace the `src` attribute of the `img` tag with the path to your profile photo. You can also update the `h1` tags with your first and last name.

    ```html
    <div class="profile-section">
        <img src="profile-photo.jpg" alt="Profile photo" class="profile-photo"> <!-- profile photo -->
        <div class="name">
            <h1>David</h1> <!-- first name or nickname -->
            <h1>Smith</h1> <!-- last name (leave blank if you don't want to provide it) -->
        </div>
    </div>
    ```

3. **Social Links**

    This section contains links to your social media profiles. You can update the `href` attributes with the URLs to your social media pages and change the text to the name of the social media platform.

    ```html
    <div class="social-links">
        <a href="#" class="social-button">Instagram</a>
        <a href="#" class="social-button">Facebook</a>
        <a href="#" class="social-button">LinkedIn</a>
        <a href="#" class="social-button">YouTube</a>
        <!-- add more social links if needed -->
    </div>
    ```

## styles.css

This file contains the styling for your webpage. Here are the key sections you might want to customize:

1. **Root Variables**

    These variables define the main colors and fonts used in your webpage. You can change these values to match your preferences.

    ```css
    :root {
        --body-bg-color: white; /* Page background */
        --card-bg-color: black; /* Card background */
        --card-text-color: white; /* Card text color */
        --button-bg-color: white; /* Button background */
        --button-hover-color: #d0d0d0; /* Button hover background */
        --main-font: 'Times New Roman', sans-serif; /* Main font */
    }
    ```

2. **Responsive Design**

    This section contains media queries to make your webpage responsive. You can adjust the values to improve the layout on different screen sizes.

    ```css
    @media screen and (max-width: 768px) {
        .card {
            width: 90%;
            padding: 2rem;
        }
        .profile-section {
            flex-direction: column;
            text-align: center;
        }
        .name {
            margin-left: 0;
            margin-top: 1rem;
        }
        .name h1 {
            display: inline;
            font-size: 1.8rem;
        }
        .social-links {
            flex-direction: column;
            gap: 1rem;
        }
        .social-button {
            width: 100%;
        }
        .profile-photo {
            width: 150px;
            height: 150px;
        }
    }
    ```

Feel free to adjust the values and add more styles as needed to match your preferences.
