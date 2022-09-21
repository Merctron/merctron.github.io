# MERCTRON: Blog, essays, and projects

Hi, I'm Murtuza. This is a collection of things I write, and work on in my spare time that is catalogued here as a living archive or for public consumption (if you find any of it interesting). This blog uses a somewhat hacky and light-weight method of publishing that makes use of [Showdown](https://showdownjs.com/) to generate HTML from markdown files like so:


```javascript
const converter = new showdown.Converter();

async function buildBlog() {
  const res  = await fetch("/path/to/file.md");
  const blog = await res.text();
  document.getElementById("blog").innerHTML += converter.makeHtml(blog);
}

buildBlog();
```

## Index

* [TEAL - A tiny text adventure engine](https://github.com/Merctron/Teal)

## About

I'm a software engineer who dabbles in writing, game development, art, and soccer among other things. If you'd like to get in touch, reach me through one of the channels listed [here](https://www.merctron.com).