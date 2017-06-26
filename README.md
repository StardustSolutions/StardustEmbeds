# Stardust Embeds
Resources for embedding Stardust reactions

Example HTML for embedding Stardust reactions:

```
<div>
  <iframe width="471" height="425" src="https://app.stardust.co/embed?playlist_id=3f9abea4-8990-461c-87b5-6c421c976cfa" frameborder="0" allowfullscreen />
</div>
```

The embedded page is responsive and has two different layouts. One for mobile (anything below 376px) and desktop (376px and above). Here is the SASS to get the proper aspect ratio for each layout:

```
div {
  position: relative;
  padding-bottom: 181.56%;
  padding-top: 35px;
  height: 0;
  overflow: hidden;
  @media (min-width: 376px) {
    position: relative;
    padding-bottom: 85%;
    padding-top: 35px;
    height: 0;
    overflow: hidden;
  }
  iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
}
```
