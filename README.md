# Block Reveal Text Animation

A scroll-triggered text animation where a colored block sweeps across each line, then peels away to reveal the copy underneath.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Live Demo](#live-demo)
- [Contributing](#contributing)
- [Contact Me](#contact-me)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/Adhamxiii/block-reveal-text-animation.git
cd block-reveal-text-animation
```

2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
npm run dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Usage

Wrap any heading or paragraph with the `Copy` component to apply the block reveal animation:

```tsx
import Copy from "@/components/Copy";

<Copy blockColor="#fe0100">
  <h1>Your headline goes here.</h1>
</Copy>

<Copy>
  <p>Body copy animates on scroll by default.</p>
</Copy>
```

### Props

| Prop | Type | Default | Description |
| --- | --- | --- | --- |
| `children` | `ReactNode` | — | Text content to animate (required) |
| `animateOnScroll` | `boolean` | `true` | Play when the element enters the viewport |
| `delay` | `number` | `0` | Delay before the animation starts (seconds) |
| `blockColor` | `string` | `"#000"` | Color of the reveal block |
| `stagger` | `number` | `0.15` | Delay between each line (seconds) |
| `duration` | `number` | `0.75` | Duration of each block sweep (seconds) |

Set `animateOnScroll={false}` to play the animation immediately on mount instead of on scroll.

## Live Demo

[View Live Demo](https://block-reveal-text-animation-psi.vercel.app/)

## Contributing

Contributions are welcome. To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m "Add your feature"`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a pull request

Please keep PRs focused and describe what changed and why.

## Contact Me

- **Email:** [adhamxiii22@gmail.com](mailto:adhamxiii22@gmail.com)
- **GitHub:** [@Adhamxiii](https://github.com/Adhamxiii)
- **LinkedIn:** [Adham Nasser](https://linkedin.com/in/adhamnasser)