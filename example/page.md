# Another page!

?> This showcases some more of Docsify's style and plugins I've mentioned

## Docsify also automatically generates the sidebar for you

It's pretty cool! It uses the `subMaxLevel` attribute in `index.html` to make these.

Just make sure you got a `_sidebar.md` file

## Adding multiple notebooks

You can add as many as you like, aslong if you provide a link in `_sidebar.md` in the root of the repo.

<!-- panels:start -->
<!-- div:left-panel -->

### A Left panel

!> Thanks to [docsify-example-panels](https://github.com/VagnerDomingues/docsify-example-panels)!

I used this extensively in my own summaries!

```js
//Code Styling supported! Copy-able thanks to https://github.com/jperasmus/docsify-copy-code
function longestString(ar) {
    const sorted = [...ar].sort((a, b) => b.length - a.length)
    return sorted[0]
}
```

<!-- div:right-panel -->

### A Right panel

> It's sometimes nice to split up your content!

<!-- tabs:start -->

##### ** Tabs! **

Made possible by [docsify-tabs!](https://jhildenbiddle.github.io/docsify-tabs)

##### ** A second tab **

They're pretty great to hide possible solutions and organise your content! Oh yeah and panels are mobile responsive

##### ** A third one! **

Hello!

<!-- tabs:end -->

#### Don't forget to

- Drink water  
- Call your grandma...

<!-- panels:end -->

## Why did I make this

I was pretty bored, and it could serve as something I could send someone if they ask me about how I make my notes.