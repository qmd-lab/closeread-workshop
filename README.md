# Closeread Workshop

Materials for a one hour workshop on using the Closeread extension for Quarto to author scrollytelling articles with data from plain markdown. Throughout the workshop, please refer to the official documentation: <https://closeread.dev/>.

## Materials

You can open the materials for this workshop in a Berkeley DataHub account by clicking the links below.

- [Open this repo in RStudio](https://stat20.datahub.berkeley.edu/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Fqmd-lab%2Fcloseread-workshop&urlpath=rstudio%2F&branch=main)

Then click on the terminal tab and change your directory to the new file of workshop materials

```bash
cd closeread-workshop
```

## Agenda

### 1. What is Scrollytelling?

Examples:

- [A Poem (and a Painting) about the Suffering that Hides in Plain Sight](https://www.nytimes.com/interactive/2022/03/06/books/auden-musee-des-beaux-arts.html)
- [MLU-Explain: Neural Networks](https://mlu-explain.github.io/neural-networks/)
- [Childhood cultural capital and adult wealth](https://mschnetzer.github.io/scrollytell_cultcap/)


### 2. Components of a Closeread

*Starting doc*: 1-components-of-closeread.qmd

*Solution*: solutions/1-components-of-closeread-solution.qmd

#### Prereqs

Two Quarto structures that Closeread takes advantage of is the fenced div and the bracketed span. Please have a look at the [Quarto docs](https://quarto.org/docs/authoring/markdown-basics.html#sec-divs-and-spans) to get a sense of how this syntax works. The syntax is also strongly inspired by the syntax for [cross-references](https://quarto.org/docs/authoring/cross-references.html).

#### Our Turn

1. Experiment with different quarto formats.
2. Instructor only: Remove `_extension` then run `quarto add qmd-lab/closeread` in this directory.
3. Switch format to `closeread-html`.
4. Add `cr-section` to encompass the image and first code cell for the table.
5. Flag image and table as stickies with `#cr-` ids.
6. Add triggers to the items with `@cr-`.
7. Change [style](https://closeread.dev/guide/styling.html).
8. Make non-`cr-section` narrower by adjusting the `grid:body-width`.

#### Your Turn

Move the second code cell for the scatterplot into the `cr-section`, make the plot a sticky, then trigger it. Also experiment with additional [styles](https://closeread.dev/guide/styling.html).

#### Our Turn Again

1. Add `.scale-to-fit`
2. Turn on debug mode


### 2. Working with Text and Code

*Starting doc*: 2-text-and-code.qmd

*Solution*: solutions/2-text-and-code.qmd

#### Our Turn

1. Create a `cr-section` for Working with Text.
2. Flag the poem as a sticky.
3. Add `.scale-to-fit`.
4. Add a trigger on the first narrative block.
5. Instead, wrap the level 2 header and the first narrative block with a div and use `focus-on` to trigger the poem.
4. Add a focus effect to the second block: `highlight="1"`.
5. Add a span id to the first reference to birth.
6. Add a focus effect to third block to highlight the span.

#### Your Turn

Create a second closeread section for the Working with Code section and treat the code block as a sticky. Split the paragraph into narrative blocks and add focus effects (highlight and zoom) to draw attention to the relevant components of the code.

#### Our Turn

1. Change the layout.

### 3. Static Graphics

*Starting doc*: 3-static-images.qmd

*Solution*: solutions/3-static-images.qmd

#### Our Turn

1. This will largely be an inspection of how to create an illusion of animation even on static graphics.


### 4. Animated Graphics

*Starting doc*: 4-animated-graphics.qmd

*Solution*: solutions/4-animated-graphics.qmd

#### Our Turn

1. Add a cr-section around the description of our big globe.
2. Set the layout to `.overlay-center`
3. Flag the plot as a sticky.
4. Create a trigger on the first narrative block.
5. Set the angle in the plot to `crTriggerProgress`.
6. Wrap the narrative blocks in a `.progress-block`.
7. Reset the angle to track `crProgressBlock`.

### Coming soon

- videos
- figure highlighting
- math