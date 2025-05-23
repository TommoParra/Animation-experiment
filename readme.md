# 🎥 SVG-Clipped Video with Magnetic Squares

A sexy little HTML/CSS/JS experiment featuring:
- A background video clipped to a custom SVG path.
- Some floating "magnetic" cards that react to your mouse.
- A frustrating hour of your life if you forget to use a local server.

## 🚨 Why your video doesn’t show up when you double-click the file

Because **browsers block video playback** (and a bunch of other things) when opening `.html` files directly via `file:///`.

If you want your `<video>` tag to work, you need to **serve the file** through a local web server.

## ✅ Easiest way: Live Server in VS Code

1. Install the [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
2. Right-click your `index.html`
3. Click **"Open with Live Server"**
4. Boom. It works at `http://localhost:5500` (or whatever port you're on)

## 🔥 Alternative: Use any local server

## Pick your poison:

### With Node (npx)
```bash
npx serve .
```

### With Python
```bash
python3 -m http.server
```

### With PHP
```bash
php -S localhost:8000
```

## 🧪 Notes
- The SVG clipPath uses objectBoundingBox, so the <path> has to be scaled correctly (already done here).

- .magneticSquare uses mousemove events to follow the pointer slightly.

- Use Chrome or Firefox. Safari always finds a way to ruin your day.
