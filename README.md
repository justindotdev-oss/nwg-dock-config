# nwg-dock-hyprland

> A minimal, glassmorphic floating dock configuration for nwg-dock on hyprland

---

## Preview

![Dock with minimal apps](https://github.com/user-attachments/assets/2e82ec9b-0ac5-4842-b817-4a7e11b0ce17)

![Dock with multiple apps](https://github.com/user-attachments/assets/6e054a4e-03cb-44fb-8461-e99127726c97)

![Full-width dock](https://github.com/user-attachments/assets/3b1dc74f-452e-4bdd-8dca-e883d5772217)

---

## Features

- **Glassmorphic Design** - Subtle transparency with blur effects
- **Smooth Animations** - 0.1s ease-out transitions on hover
- **Lift Effect** - Buttons visually lift when hovered
- **Minimal Aesthetic** - Clean borders and subtle shadows
- **Responsive Layout** - Adapts to content width automatically

---

## Installation

### Prerequisites

- [nwg-dock](https://github.com/nwg-piotr/nwg-dock) installed
- Hyprland window manager

### Setup

1. **Clone this repository**

   ```bash
   git clone https://github.com/justindotdev-oss/nwg-dock-config.git
   cd nwg-dock-config
   ```

2. **Copy the CSS file to nwg-dock config directory**

   ```bash
   cp style.css ~/.config/nwg-dock/
   ```

3. **Making it toggle-able with the `Super` key**

Add this line to your hyprland `*.conf` file:
`bindr = SUPER, Super_L, exec, pkill nwg-dock-hyprla || nwg-dock-hyprland -i 30 -nolauncher -mb 3 -mt 3 -x
`

---

## Customization

### Animation Speed

Adjust the transition timing:

```css
button {
  transition: all 0.1s ease-out; /* Change 0.1s for faster/slower */
}
```

### Border Radius

Modify the dock roundness:

```css
#box {
  border-radius: 14px; /* Increase for more rounded, decrease for sharper */
}
```

---
