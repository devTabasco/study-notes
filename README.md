# Study Notes Website

This is my personal study notes website where I share what I'm learning. I set it up so that when I write notes in Markdown, they automatically get converted to HTML and appear on the website.

## 🌐 Website

[https://devtabasco.github.io/study-notes/](https://devtabasco.github.io/study-notes/)

## 📚 How I Organized It

```
.
├── posts/              # Where I keep my markdown notes
├── posts_html/         # Where the HTML versions go
├── assets/
│   └── css/           # My website styles
├── template.html      # The template I use
└── index.html        # The main page
```

## 📝 My Writing Process

I write my study notes like this:

1. Write a new note in markdown (in `posts/`)
2. Format it in markdown
3. Add it to the homepage
4. Push it to GitHub

Here's how I structure my notes:
```markdown
# Study Note Title

## Section 1
Content...

## Section 2
Additional content...
```

## ✨ How I Built It

I put this together using:
- Pandoc for converting my notes
- GitHub Actions to automate everything
- GitHub Pages to host it 