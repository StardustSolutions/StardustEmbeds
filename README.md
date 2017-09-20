# Stardust Embeds
Resources for embedding Stardust reactions

Example HTML for embedding Stardust reactions:

```
<section>
  <div>
    <iframe width="380" height="700" src="https://app.stardust.co/embed_v2?reaction_id=3f9abea4-8990-461c-87b5-6c421c976cfa" frameborder="0" allowfullscreen />
  </div>
  <!-- add additional embeds here -->
</section>
```

The embedded page is responsive, however, you will need to make sure the iframe it's contained in is responsive on your website. Here is the SASS to get the iframe to be responsive:

```
section {
  max-width: 380px;
  div {
    position: relative;
    padding-bottom: 181.56%;
    padding-top: 10px;
    height: 0;
    overflow: hidden;
    iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
    }
  }
}
```
