# Closeread Workshop

Materials for a one hour workshop on using the Closeread extension for Quarto to author scrollytelling articles with data from plain markdown. Throughout the workshop, please refer to the official documentation: <https://closeread.dev/>.

## Agenda

### 1. What is Scrollytelling?

Examples:

- [A Poem (and a Painting) about the Suffering that Hides in Plain Sight](https://www.nytimes.com/interactive/2022/03/06/books/auden-musee-des-beaux-arts.html)
- [MLU-Explain: Neural Networks](https://mlu-explain.github.io/neural-networks/)
- [Childhood cultural capital and adult wealth](https://mschnetzer.github.io/scrollytell_cultcap/)


### 2. Components of a Closeread

*Starting doc*: components-of-closeread.qmd
*Solution*: solutions/components-of-closeread-solution.qmd

#### Our Turn

1. Experiment with different quarto formats.
2. Instructor only: Remove `_extension` then run `quarto add qmd-lab/closeread` in this directory.
3. Switch format to `closeread-html`.
4. Add `cr-section`.
5. Flag a few items as stickies with `#cr-` ids.
6. Add triggers to the items with `@cr-`.
7. Change styles.

#### Your Turn

1. Change more styles.
2. Create second `cr-section`.

#### Our Turn Again

1. Turn on debug mode


### 2. Working with Text and Code

*Starting doc*: text-and-code.qmd
*Solution*: solutions/text-and-code.qmd

#### Our Turn

1. Flag the poem as a sticky.
2. Add `.scale-to-fit`
3. Add a trigger on the first narrative block.
4. Add a focus effect to the second block: `highlight="1"`.
5. Add a span id to a phrase.
6. Add a focus effect to third block to highlight the span.

#### Your Turn

Create a second closeread section for the second half of the document and treat the code as a sticky. Add focus effects (highlight and zoom) and change the layout and styles to differentiate the second section.



To be added:
-  static-images.qmd (encompassing things from minard and build a plot + pan and zoom)
-  animated-graphics.qmd (ojs)
- Coming soon:
  - videos
  - figure highlighting
  - math