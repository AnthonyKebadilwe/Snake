# 🐍 Snake

An animated snake that eats my GitHub contribution graph. It is generated automatically with GitHub Actions and updates every day.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/AnthonyKebadilwe/Snake/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/AnthonyKebadilwe/Snake/output/github-snake.svg" />
  <img alt="github-snake" src="https://raw.githubusercontent.com/AnthonyKebadilwe/Snake/output/github-snake.svg" />
</picture>

## How it works
- A GitHub Actions workflow (`.github/workflows/snake.yml`) reads my contribution graph.
- It generates light and dark SVG animations of a snake eating the contributions.
- The images are saved to the `output` branch and refreshed every 24 hours, or whenever I push or run the workflow manually.

## Use it on your own profile
1. Copy `.github/workflows/snake.yml` into your own repo.
2. Go to **Settings > Actions > General** and set workflow permissions to **Read and write**.
3. Run the workflow from the **Actions** tab.
4. Embed the generated SVG in your README.

## Built with
- [Platane/snk](https://github.com/Platane/snk) – snake generator
- GitHub Actions
