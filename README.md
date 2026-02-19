## Storybook Usage Instructions By Herlan Mustopa

This project uses **Storybook** to technical test in Makyo Co.

---

### **1. Installing**

If Storybook is not already installed in your project, you can add it by running:

```bash
npx storybook@latest init
```

This command will:

- Configure Storybook for your project.
- Add the necessary dependencies and scripts to your `package.json`.

---

### **2. Running**

To start the Storybook development server, run:

```bash
npm run storybook
```

Once started, Storybook will open automatically in your default browser. If it doesn’t, you can manually access it at:

```
http://localhost:6006
```

---

### **3. Component Stories**

The stories for the `Dropdown` component are located in:

```bash
src/components/Dropdown.stories.tsx
```

### **4. Component features**

In Storybook:

1. Navigate to the `Dropdown` component story under the **Dropdown** section.
2. Use the **Controls** panel to dynamically adjust props like:
   - **`label`**: Customize the label text.
   - **`multiple`**: Enable or disable multiple selection.
   - **`outlined`**: Toggle the outlined style.
   - **`withSearch`**: Enable or disable the search bar.
3. Interact with the dropdown and observe the real-time changes.

### **5. Building Storybook for Deployment**

To build Storybook for production deployment, run:

```bash
npm run build-storybook
```

This will generate a `storybook-static` folder in your project root. You can deploy this folder to any static hosting platform like **Vercel**, **Netlify**, or **GitHub Pages**.

---

### **6. Troubleshooting**

If you encounter issues:

- **Storybook fails to start**: Ensure all dependencies are installed correctly.
- **Component does not render**: Verify that the story file is named correctly (\*.stories.tsx) and that components are imported properly.
- **Props not updating**: Check that argTypes are defined correctly in the story file.

---

Now you’re ready to use Storybook to test and explore your `Dropdown` component!
