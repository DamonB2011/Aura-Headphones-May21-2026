# What it is

It's a brand new, fully front-end idea landing page I've created for a luxury headphone company. It's the 5th project I've made to date, and it's the 1st I've ever built exclusively with HTML/CSS/JS, without a single frame. The main goal of the project was to create a truly scroll-driven and interactive experience. Think of the page as a microsite rather than a traditional marketing page-more of an Apple-esque experience. Designed in Claude Design, built from scratch, and hosted via Vercel.

---

## How It Works

The site is delivered in a single HTML file. There's no build pipeline and no external libraries to be installed; the entire page can just be opened directly in the browser. No npm. No node_modules. None.

- **SnapScroll** - I've implemented a CSS scroll-snap-type property of 'y mandatory'. This makes the page scroll down like a flip-book, and each section acts as a distinct 'page' with a unique feel. I ended up with twelve of these pages.
- **RevealAnimations** - When one of these pages snaps into view, its contents smoothly fade and animate in. Everything starts hidden, with slight vertical displacement, before gracefully animating into its final position with subtle timing delays.
- **3DHeadphoneModels** - The page incorporates two 3D headphone models powered by Spline. In the Hero, I've implemented an interactive color changer so you can change colors with a drag, and in the Immerse section, you can get a full view of the product in 3D.
- **CustomCursor** - A glowy blue dot is used as a cursor, with a slight trailing ring behind it. The cursor gets slightly larger when it hovers over any interactive elements.
- **ANCVisualizer** - The ANC section contains forty individual bars which move upward from the bottom to simulate sound being blocked.
- **SpatialAudioVisualizer** - To visually demonstrate the 3D audio, six dots of different sizes and speed orbit around a central point.
- **KeyboardNavigation** - The entire page is fully navigable via your arrow keys, Page Up/Down, Home, and End keys.
- **NavigationDots** - On the right side of the screen, a number of dots shows you which page of the site you are currently on, along with tooltips when you hover over them.

---

## Sections

1. Hero:Interactive 3D headphone color changer, compelling headlines and calls to action.
2. Features:Highlights of the key selling points:40-hour battery life, ANC Pro, Hi-Res Audio.
3. Immerse:A spatial audio-immersive 3D view of the headphone.
4. ANC:A visual representation of Active Noise Cancellation, where noise gets absorbed by a block of bars.
5. SpatialAudio:A more abstract visual demonstration of sound.
6. Battery: A simple and visually engaging battery animation to indicate usage.
7. Materials:Displays textures of aluminium and leather materials to communicate quality.
8. Specs:Contains all technical specifications such asdriver size,frequency response,impedance,weight, andBluetoothversion.
9. Testimonial 01
10. Testimonial 02
11. Testimonial 03
12. Final Call to Action: A purchaseCTA button to end the journey.

---

## TechStack

| Layer | Detail |
| :--------------------- | :-------------------------------------------------------------- |
| Markup | HTML5 |
| Styling |Vanilla CSS with custom properties. |
| Animation | CSS transitions and vanilla JavaScript (IntersectionObserver API). |
| 3D scenes |Spline embed(via iframes). |
| Fonts | Syne, DM Sans and JetBrains Mono (allvia Google Fonts). |
| Deployment |Vercel. |

---

## KeyTakeaways

Working on a 100% front-end-only project like this without a single line of code related toReactor any sort of build pipeline was incredibly liberating. Everything from the snap scroll to the custom cursor and all the various animated effects(which leveraged browser APIs like the IntersectionObserver) runs entirely within the browser, no node_modules whatsoever. There were challenges to overcome with making the IntersectionObserver calls to reveal sections super smooth, as well as getting the ANC animation to look natural and satisfying.
