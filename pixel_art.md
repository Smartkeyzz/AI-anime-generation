# How to Make Pixel Art with Tsubaki.3 on PixAI: A Practical Prompting Workflow

Pixel art looks simple at first glance, but getting an AI image generator to produce convincing pixel-style artwork takes more than adding the words *pixel art* to a prompt.

The model also needs clues about the visual treatment you want: blocky shapes, stepped edges, simplified shading, grouped colors, and a limited-looking palette.

![Image description](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/2kc9gsbpc134o0b00dhk.png)

In this tutorial, I’ll use **Tsubaki.3 on [PixAI](https://eap.pixai.art/go/rhoda2)** to create a full-body pixel-style character from text. I’ll start with a reusable prompt template, compare it with a much simpler prompt, and then adjust the wording to see how far the model can be pushed toward a more traditional retro-game appearance.

The goal here is **pixel-style character illustration**, not a technically prepared game sprite. If you need an exact sprite resolution, transparent background, animation sheet, or tile-ready asset, additional editing may still be necessary. 

## Step 1: Select Tsubaki.3

Open [PixAI's image generation interface](https://eap.pixai.art/go/rhoda2) and select **Tsubaki.3** as the model.

For this experiment, I kept the generation setup simple because I wanted the prompt wording to do most of the work.

My setup was:

* **Model:** Tsubaki.3
* **Image size/aspect ratio:** 3:5
* **Other settings changed:** None

![Image description](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/y78ku4tmqeq8mqlg68m9.jpg)

![Image description](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/znwjz8pwdlvmpn5npcym.jpg)


Use the exact settings visible in your current PixAI interface rather than relying on older screenshots or instructions.

Once the model is selected, the next step is building the [prompt](https://blog.pixai.art/en/tsubaki-3-prompt-guide/).

## Step 2: Start With a Reusable Pixel-Art Prompt

Instead of writing a completely new prompt every time, I used a template where the character details can be swapped while the style instructions remain consistent.

```text
Pixel art illustration of [character type], full body, [hairstyle and hair color], [clothing and accessories], [pose or action]. Centered on a plain [background color] background. Retro 2D RPG character aesthetic, clearly visible square pixel blocks, crisp stair-stepped outlines, flat color clusters, limited color palette, minimal shading, simple readable silhouette. No text.
```

The important part is the second half of the prompt.

Terms such as **stair-stepped outlines**, **flat color clusters**, **limited color palette**, and **minimal shading** give the model more information about what kind of pixel-style treatment you are expecting. 

For my first character, I used a fantasy courier:

```text
Pixel art illustration of a young female fantasy courier, full body, short dark-red bob hair, cream tunic, brown shorts, ankle boots, and a small green shoulder bag, standing while holding a folded letter. Centered on a plain pale beige background. Retro 2D RPG character aesthetic, clearly visible square pixel blocks, crisp stair-stepped outlines, flat color clusters, limited color palette, minimal shading, simple readable silhouette. No text.
```
![Image description](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/lu4p4i9x9n9vwz2klxxh.png)

I deliberately kept the character design straightforward.

There is one character, a clear full-body pose, only a few accessories, and a plain background. This gives the model less unnecessary detail to handle and makes it easier to judge the pixel treatment.

## Step 3: Generate and Inspect the Result

After generating the image, I checked two things separately:

1. Did the model follow the character description?
2. Did the image actually look pixel-styled?

The first result followed the character description closely. The short dark-red hair, cream tunic, brown shorts, boots, green shoulder bag, and folded letter were all visible.

![Image description](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/ggclgp6k64hwe6zat8c9.png)

The pixel treatment was also noticeable.

The edges around the hair, clothing, boots, and accessories were not completely smooth. Many of the contours had a stepped appearance, while the colors were grouped into more obvious blocks instead of using highly blended anime-style rendering. 

However, the result was still fairly detailed.

The face, hair, hands, and folds in the clothing contained more detail than you would normally expect from a very low-resolution traditional sprite.

That distinction matters.

The image looks like **pixel art**, but it is still an AI-generated pixel-style illustration rather than artwork built manually on a fixed low-resolution pixel grid. 

## What Does the Pixel Treatment Look Like Up Close?

Zooming into the image makes the effect easier to see.

Around the hair and clothing, curves are represented using more visible stepped edges. Colors also appear in grouped areas rather than smoothly transitioning across every surface.

That visual effect is what the prompt is trying to encourage.

![Image description](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/5uiidj5nr4qkjey1r823.jpg)

It does **not** mean the model is guaranteeing a particular sprite resolution, exact pixel grid, or fixed number of colors.

The prompt influences the appearance. It does not enforce technical sprite specifications.

## Does the Detailed Prompt Actually Matter?

To test that, I generated the same character again with most of the style instructions removed.

The simpler prompt was:

```text
Pixel art illustration of a young female fantasy courier, full body, short dark-red bob hair, cream tunic, brown shorts, ankle boots, and a small green shoulder bag, standing while holding a folded letter. Centered on a plain pale beige background. No text.
```

![Image description](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/rckyme7i7njva0owff5b.png)

I kept the character and background the same so that the main variable was the pixel-art wording.

In this test, simply including **“pixel art illustration”** was already enough for Tsubaki.3 to move the output toward a pixel-style appearance.

However, the basic version looked slightly closer to a polished anime illustration with a pixel-like treatment.

The longer prompt gave the result a stronger retro RPG feel. The difference was not huge, but the outlines, color grouping, and simplified forms looked more intentional. 

## What Each Pixel-Art Prompt Phrase Does

The extra wording serves different purposes:

* **Clearly visible square pixel blocks** pushes the image toward a visibly block-based treatment.
* **Crisp stair-stepped outlines** discourages completely smooth curves.
* **Flat color clusters** encourages larger grouped areas of color.
* **Limited color palette** reduces excessive color variation.
* **Minimal shading** discourages complex lighting and gradients.
* **Simple readable silhouette** keeps the character shape easy to recognize.

None of these phrases guarantees a particular result on every generation.

They simply give the model more explicit visual direction.

## Step 4: Push the Result Toward a More Traditional Pixel Look

My first result already looked convincingly pixel-styled, so instead of pretending something was wrong with it, I made one targeted change.

I added:

```text
Larger visible pixel blocks, simpler shading, fewer fine details.
```

The updated prompt became:

```text
Pixel art illustration of a young female fantasy courier, full body, short dark-red bob hair, cream tunic, brown shorts, ankle boots, and a small green shoulder bag, standing while holding a folded letter. Centered on a plain pale beige background. Retro 2D RPG character aesthetic, clearly visible square pixel blocks, crisp stair-stepped outlines, flat color clusters, limited color palette, minimal shading, simple readable silhouette, larger visible pixel blocks, simpler shading, fewer fine details. No text.
```

![Image description](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/9p7lz2zn2zs76rfunk96.png)

The change helped, although only slightly.

The hair and clothing edges looked a little more blocky, while some of the finer clothing details were reduced.

It moved the result closer to a retro game-style illustration without completely changing the image. 

That is also a useful reminder when working with generative models: prompt edits do not always produce dramatic changes.

Sometimes the difference is subtle.

## A Simple Troubleshooting Approach

If your output looks too smooth, try adding:

```text
Larger visible pixel blocks, simpler shading, fewer fine details.
```

If the result becomes too busy, simplify the clothing and remove unnecessary accessories.

If the background distracts from the character, use a plain background and add:

```text
No additional background objects.
```

The best approach is to change **one variable at a time**.

That way, you can actually tell which wording affected the result rather than rewriting the whole prompt after every generation. 

## Step 5: Create a Different Character With the Same Style

Once the style wording was working, I reused it for a second character instead of rebuilding the prompt from scratch.

This time, I created an apprentice alchemist:

```text
Pixel art illustration of a young male apprentice alchemist, full body, messy dark blue hair, light tunic, short brown cape, dark trousers, boots, and a small belt pouch, holding a small bottle. Centered on a plain pale gray-blue background. Retro 2D RPG character aesthetic, clearly visible square pixel blocks, crisp stair-stepped outlines, flat color clusters, limited color palette, minimal shading, simple readable silhouette. No text.
```
![Image description](https://dev-to-uploads.s3.us-east-2.amazonaws.com/uploads/articles/8su8cgb7ucro4mz6dfyz.png)

The character changed, but the visual rules stayed the same.

The new result still had recognizable block-like outlines and grouped colors, even though details such as the blue hair, cape, pouch, and bottle were completely different from the original courier.

This is the real benefit of having a reusable template: once you find style wording that works reasonably well, you can keep it and replace only the character-specific details. 

## Exporting the Final Image

Once you're happy with the result, save the generated image and record its actual export information.

For example:

```text
File format: PNG
Dimensions: 1104 x 1824
```

Do not guess these values. Check the actual downloaded file.

Also keep the intended use in mind.

An AI-generated pixel-style image can work well for:

* character concepts
* profile images
* visual references
* social posts
* pixel-style illustrations

But it should not automatically be treated as a production-ready game sprite.

A game asset may still need resizing, transparency cleanup, palette control, sprite-sheet preparation, or manual pixel editing. 

## Conclusion

Creating pixel-style characters with Tsubaki.3 is less about finding one magical prompt and more about giving the model clear visual constraints.

The workflow I used was:

**Select Tsubaki.3 → Fill in the template → Generate → Inspect the result → Adjust one detail → Reuse the style**

The basic prompt showed that Tsubaki.3 can already respond to the phrase *pixel art illustration*, but the more detailed version gave me better control over things like stepped outlines, color grouping, shading, and overall retro styling.

And when I wanted the result to move slightly closer to a traditional pixel-art appearance, adding **“larger visible pixel blocks, simpler shading, fewer fine details”** gave me a practical adjustment without having to rewrite the entire prompt.

Once you have a style description that works, keep it.

Change the character, pose, clothing, accessories, or background instead—and use each generation to refine the visual direction a little further. 
