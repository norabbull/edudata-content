# Content for [EduData.no](https://edudata.no)

Open-source content for education and research.

Feel free to contribute by contacting [Morten Munthe](mailto:morten.munthe@nmbu.no?subject=EduData%20Contribution) or by [creating a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).

## Folders explained

- `📁 .github`  
Ignore this. It does magic.
- `📁 data`  
Temporary data storage solution  
_Note: This folder will be published to [EduData.no](https://edudata.no)_
- `📁 private`  
Hidden notebooks for internal use or drafts  
_Note: The code is still publically available on GitHub, but it's not published to [EduData.no](https://edudata.no)_
- `📁 public`  
Notebooks to publish to [EduData.no](https://edudata.no)

## Guidelines

Look at the published notebooks for inspiration.

#### Follow Markdown conventions

See GitHub's [Mastering Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) guide.

If you must use HTML, keep it simple and standalone from Markdown elements, e.g.:

This is perfect:  ✅😄

```markdown
# Heading

Paragraph with a [link](https://edudata.no).

<div>
  <p>Some HTML</p>
</div>
```

This should be avoided:  ❌😢

```markdown
# Head<span style="color: 'red'">in</span>g

Paragraph with a **bold <a href="https://edudata.no">link</a>**.

> **Note:** This is a blockquote
> 
> <div>
>  <p>Some HTML</p>
> </div>

```



#### Folder name and `.ipynb` file name must match

- `📁 et-solid-opplegg`
  - `📄 et-solid-opplegg.ipynb` ✅😄
- `📁 et-solid-opplegg`
  - `📄 Et uheldig eksempel.ipynb` ❌💀

#### Use copyright free media

- [Stable Diffusion](https://huggingface.co/spaces/stabilityai/stable-diffusion)
  - Generate free AI images
- [PixaBay](https://pixabay.com/)
  - Royalty free images, illustrations, vectors, videos, music and sound effects
- [Pexels](https://www.pexels.com/)
  - Royalty free images and videos
- ...or create your own 😊

#### Add a `metadata.json` file to each notebook-folder

- `📁 eksempel`
  - `📄 eksempel.ipynb`  
  - `📄 metadata.json` ✅😄  
    ```json
    {
      "title": "Eksempel",
      "description": "Dette er et eksempel.",
      "tags": [{ "tag": "fag", "color": "orange" }],
      "image": "https://pixabay.com/photos/cat-pet-licking-animal-tabby-cat-323262/"
    }
    ```
    - Colors for tags (optional):  
      - Available colors: https://mantine.dev/theming/colors/#default-colors  
      - Examples: `pink`, `green.0`, `blue.9`, `gray`, `cyan.0`

#### Use lowercase file extensions

- `cat-with-a-hat.png` ✅😄
- `cat-with-a-hat.PNG` ❌💀
- It's a limitation of GitHub, and it gets messy if we don't.

#### Avoid special characters in filenames

- `æøå er  $ærdeles norske #symboler?!.png` ❌💀
- `aeooaa-er-saerdeles-norske-symboler.png` ✅🙂
- `norske-symboler.png` ✅😄
- It hasn't caused big problems yet, but it'll probably save us some headaches in the future.
