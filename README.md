🎡 Word Circle Interactive Template

An interactive UI component featuring a centralized "Word Circle" navigation hub designed for engaging, non-linear content discovery. This project pairs orbital imagery with a dynamic central display, allowing users to reveal specific information through a "Click-and-Reveal" mechanic.

🚀 Live Demo

Explore the Interactive Template Here

✨ Project Overview

This interactive component replaces standard tabs with a sleek, circular navigation hub. It is specifically designed to associate bold imagery with concise descriptive text, making it an ideal choice for educational modules, feature showcases, or interactive storytelling.

Key Features

Central Navigation Hub: A primary "Center Circle" that serves as the dynamic display area for revealed information.

Orbital Content Nodes: Interactive outer circles that orbit the center. Each node contains a sequence number, high-resolution imagery, and a hidden text payload.

Smart Click-and-Reveal: Clicking any orbital node dynamically updates the central text content while applying an "active" state highlight to the selected node.

Hover Overlays: Nodes feature a sophisticated overlay that reveals a title and sequence number upon hovering, providing immediate visual feedback.

Responsive Geometric Layout: Leverages CSS media queries and viewport units to ensure the circular UI remains balanced and functional across mobile, tablet, and desktop screens.

🛠️ Technical Implementation

Mathematical Positioning: The orbital nodes are positioned using JavaScript trigonometry ($Math.cos$ and $Math.sin$) to calculate $(x, y)$ coordinates. This ensures perfectly equal distribution around the center regardless of the number of nodes.

Modern Styling: Powered by Tailwind CSS and custom CSS variables, the UI utilizes a professional palette:

Midnight Blue (#1f2a52): Used for primary grounding and text.

Accent Cyan (#00bec7): Highlights interactive elements and active states.

Light Aqua (#d2f0f0): Provides a clean, modern background aesthetic.

Vanilla JS Interaction: A lightweight script manages the state, updating the central DOM element and handling the transition of active classes without external dependencies.

📂 Project Structure

Four-image_Word-Circle_Click-and-Reveal/
├── index.html          # Main application (UI, Styles, and Logic)
├── previews/           # Auto-generated social preview assets
└── .github/workflows/  # CI/CD for thumbnail generation


⚙️ Customization

To swap out content, update the data-text attribute and the image sources within the outer-circle divs in index.html:

<div class="outer-circle" data-text="Your hidden information here...">
  <img src="your-image.jpg" alt="Description">
  <div class="hover-content-overlay">
    <div class="circle-number">1</div>
    <h3>Your Topic Heading</h3>
  </div>
</div>


🤖 Automation & Catalog Integration

This repository includes a GitHub Actions workflow that automatically captures a high-resolution screenshot of the UI. This preview is then synchronized with the Catalog of Repos to provide an up-to-date visual gallery of all active projects.

📄 License

MIT License - Created for the accounts-eles ecosystem.
