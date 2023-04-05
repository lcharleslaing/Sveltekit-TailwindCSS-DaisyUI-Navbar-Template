# SvelteKit-TailwindCSS-DaisyUI-Navbar-Template

This is a starter template for building modern web applications using SvelteKit, Tailwind CSS, and DaisyUI. It comes with a responsive and customizable navbar, pre-built pages, and various UI components to kickstart your project. The template also includes support for authentication and user management.

## Features

- SvelteKit for building web applications
- Tailwind CSS for styling
- DaisyUI for UI components
- Responsive and customizable navbar
- Pre-built pages for common use cases
- UI components for rapid development
- Authentication and user management

## Bonus

```bash
npx sveltekit-page-title-component
```

This package adds `PageTitle.svelte` to all routes with a `+page.svelte` within it that names the page based on the `Page URL`

## Getting Started

### Prerequisites

- Node.js v14.x or later
- npm v6.x or later
- Use .env file to store the Website name (VITE_SITE_NAME="Your Site Name")

.env

```bash
VITE_SITE_NAME="Your Site Name"
```

### Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/Sveltekit-TailwindCSS-DaisyUI-Navbar-Template.git
```

2. Navigate to the project folder:

```bash
cd Sveltekit-TailwindCSS-DaisyUI-Navbar-Template
```

3. Install the dependencies:

```bash
npm install
```

4. Run the development server:

```bash
npm run dev
```

5. Open your browser and visit <http://localhost:3000>.

## Building for Production

To build the application for production, run the following command:

```bash
npm run build
```

This will create a `dist` folder with the compiled assets, which can be deployed to your preferred hosting provider.

## Customizing the Template

You can customize the template by modifying the components in the `src/lib/components` folder and adding your own styles in `src/app.postcss`. The pre-built pages can be found in the `src/routes` folder, and you can add new pages by creating additional Svelte components inside the folder.

For authentication and user management, you can modify the `src/routes/auth` folder and integrate it with your preferred authentication provider.

## Contributing

Contributions are welcome! If you have any ideas, suggestions, or bug reports, feel free to submit an issue or create a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [SvelteKit](https://kit.svelte.dev/)
- [Tailwind CSS](https://tailwindcss.com/)
- [DaisyUI](https://daisyui.com/)
