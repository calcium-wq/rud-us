# rud-us
rudeus ifodqhfdqmhldqhomdhgofdùqoufldjùqJDFQ

## Dark mode toggle

Use this button to switch a page between light and dark mode:

```html
<button id="theme-toggle" type="button" aria-pressed="false">
  Toggle dark mode
</button>

<script>
  const toggle = document.getElementById("theme-toggle");

  toggle.addEventListener("click", () => {
    const isDark = document.documentElement.classList.toggle("dark-mode");
    toggle.setAttribute("aria-pressed", String(isDark));
  });
</script>
```

```css
:root {
  color-scheme: light;
  background: #ffffff;
  color: #111111;
}

:root.dark-mode {
  color-scheme: dark;
  background: #111111;
  color: #ffffff;
}
```
