# SETUP.md

## 8-step setup guide (English + Persian)

### English
1. Create a public repository with the exact name of your GitHub username, for example: `amirtt99/amirtt99`.
2. Open the repository and go to the `Settings` tab.
3. In the left menu, click `Actions` and enable GitHub Actions for the repo.
4. Create the `.github/workflows/snake.yml` file as shown in this repository.
5. Commit and push the file to the default branch (`main`).
6. Open the Actions tab and run the workflow manually once using `workflow_dispatch`.
7. Wait for the workflow to finish; it will generate SVG files in the `output` branch.
8. Add the generated SVGs to your `README.md` using the raw GitHub URLs.

### فارسی
1. یک ریپوی عمومی با نام دقیق یوزرنیم خود بسازید؛ مثلاً: `amirtt99/amirtt99`.
2. به تب `Settings` در ریپو بروید.
3. از منوی سمت چپ، گزینه `Actions` را باز کنید و GitHub Actions را فعال کنید.
4. فایل `.github/workflows/snake.yml` را مثل نمونه داخل این ریپو بسازید.
5. فایل را commit و push کنید روی شاخه اصلی (`main`).
6. در تب Actions، یک‌بار به صورت دستی workflow را اجرا کنید.
7. صبر کنید تا workflow تمام شود؛ فایل‌های SVG روی شاخه `output` ساخته می‌شوند.
8. لینک‌های raw SVG را در `README.md` اضافه کنید.

## URLs to replace when username changes

- `https://github.com/amirtt99` → replace with your username.
- `https://raw.githubusercontent.com/amirtt99/amirtt99/output/github-snake.svg` → replace `amirtt99` and repo name.
- `https://raw.githubusercontent.com/amirtt99/amirtt99/output/github-snake-dark.svg` → replace `amirtt99` and repo name.
- `https://github-readme-stats.vercel.app/api?...username=amirtt99` → replace `amirtt99` with the new username.
- `https://github-profile-trophy.vercel.app/?username=amirtt99` → replace `amirtt99` with the new username.
- `https://komarev.com/ghpvc/?username=amirtt99` → replace `amirtt99` with the new username.

## GitHub Markdown limits and notes

- GitHub strips raw `<style>` blocks from `README.md`.
- You can use safe HTML such as `<div align="center">`, `<img>`, `<picture>`, and tables.
- Inline CSS inside SVGs is allowed and works; inline CSS in Markdown HTML is usually ignored.
- Avoid extremely wide ASCII banners or large blocks of code that break mobile layout.
- Keep widget URLs valid and use the correct username everywhere.
- Some dynamic widgets require the repo to be public and the service to allow the request.
- `README.md` should remain readable and fast to scan in under 10 seconds.

## Reference note for Snake

Use the following pattern in your profile README:

```md
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/USERNAME/USERNAME/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/USERNAME/USERNAME/output/github-snake.svg" />
  <img alt="GitHub Snake" src="https://raw.githubusercontent.com/USERNAME/USERNAME/output/github-snake.svg" />
</picture>
```

Replace `USERNAME` with your GitHub username.
