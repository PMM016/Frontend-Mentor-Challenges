# Social Links Profile

This is a simple social links profile card built with HTML, CSS, and JavaScript. It displays personal information and links to various social media platforms.

## Preview

![Preview](https://res.cloudinary.com/dz209s6jk/image/upload/f_auto,q_auto,w_700/Challenges/sfsa14rwjz0wp7lzel2x.jpg)

## Features

- Responsive design for mobile and desktop.
- Hover effects on social links.
- Customizable personal details.

## Technologies Used

- HTML5
- CSS3 (with CSS variables for colors)
- JavaScript (minimal, for logging)

## Installation

1. Clone the repository: Git clone https://github.com/PMM016/Frontend-Mentor-Challenges,git
2. Open `index.html` in your browser.

## Customization

- Update the name, location, quote, and links in the `index.html` file.
- The avatar image can be replaced by updating the `src` attribute in the `<img>` tag.

## Credits

- Challenge from [Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32EgF6ls).
- Fonts from [Google Fonts](https://fonts.google.com/specimen/Inter).

## Author

- Name: PMM016

``` HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <title>Social Links Profile</title>
    <style>
        :root {
            --green: hsl(75, 94%, 57%);
            --white: hsl(0, 0%, 100%);
            --grey: hsl(0, 0%, 20%);
            --dark-grey: hsl(0, 0%, 12%);
            --off-black: hsl(0, 0%, 8%);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--off-black);
            color: var(--white);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            font-size: 14px;
        }

        .card {
            background-color: var(--dark-grey);
            padding: 2.5rem 2.5rem 2rem;
            border-radius: 0.75rem;
            max-width: 327px;
            width: 100%;
            text-align: center;
        }

        .avatar {
            width: 88px;
            height: 88px;
            border-radius: 50%;
            margin-bottom: 1.5rem;
        }

        .name {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 0.25rem;
        }

        .location {
            color: var(--green);
            font-weight: 700;
            margin-bottom: 1.5rem;
        }

        .quote {
            font-weight: 400;
            margin-bottom: 1.5rem;
        }

        .links {
            list-style: none;
        }

        .link-item {
            margin-bottom: 1rem;
        }

        .link {
            display: block;
            background-color: var(--grey);
            color: var(--white);
            text-decoration: none;
            padding: 0.75rem;
            border-radius: 0.5rem;
            font-weight: 700;
        }

        .link:hover {
            background-color: var(--green);
            color: var(--off-black);
        }

        @media (min-width: 376px) {
            .card {
                max-width: 384px;
            }
        }
    </style>
</head>
<body>
    <main class="card">
        <img src="https://api.dicebear.com/7.x/avataaars/svg?seed=PMM" alt="PMM" class="avatar">
        <h1 class="name">PMM</h1>
        <p class="location">Location, Country</p>
        <p class="quote">"Your profession or quote here."</p>
        <ul class="links">
            <li class="link-item"><a href="https://github.com/" class="link">GitHub</a></li>
            <li class="link-item"><a href="https://www.frontendmentor.io/" class="link">Frontend Mentor</a></li>
            <li class="link-item"><a href="https://www.linkedin.com/" class="link">LinkedIn</a></li>
            <li class="link-item"><a href="https://twitter.com/" class="link">Twitter</a></li>
            <li class="link-item"><a href="https://www.instagram.com/" class="link">Instagram</a></li>
        </ul>
    </main>
    <script>
        // No JavaScript is required for this static profile card, but here's a simple script if needed.
        console.log("Social links profile loaded.");
    </script>
</body>
</html>
```
