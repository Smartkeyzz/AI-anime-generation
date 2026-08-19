# How I Created a Spider-Man SSR Gacha Screen with PixAI Studio
Spider-Man seems almost made for a character-based game. He has an instantly recognizable suit, iconic abilities, and countless versions that could easily fill an entire character roster. But what would he look like as a limited SSR character in a fictional gacha game?

I decided to explore that idea using PixAI Studio’s existing Fated Pull workflow, a template built to transform character artwork into a mobile-game-style gacha result screen. Rather than creating the entire interface from scratch, I cloned the workflow, generated my Spider-Man artwork with Tsubaki.3 inside Studio, replaced the original character, and used the existing setup to produce the final SSR-style reveal.

In this tutorial, I’ll walk through the process step by step and show how you can adapt the same workflow to create your own character concepts.

Please refer here for images: https://substackcdn.com/image/fetch/$s_!xcsU!,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2Fff57b26a-7d24-41c2-8df7-4022332b61f7_800x1333.png

## The PixAI Studio Workflow I’m Using

Rather than building the gacha screen from individual nodes, I started with an existing PixAI Studio template. PixAI includes “Fated Pull” Gacha Pull Screen | Make Your Character a Limited SSR, a workflow that already has the basic structure needed to transform character artwork into an SSR-style game reveal.

I found the Fated Pull workflow through PixAI’s “How to Use PixAI Studio: From Character Photoshoots to AI Animation, 10 Templates You Can Clone Instantly” guide. From there, I selected Clone this template now, which opened the corresponding A Draw of Fate workspace in PixAI Studio.

This gave me a practical starting point. Instead of rebuilding the workflow myself, I could focus on replacing the existing character with Spider-Man and adapting the template to fit the concept I had in mind.

## Step 1: Open the Fated Pull Workflow in PixAI Studio

The first step is to open the Fated Pull workflow in PixAI Studio. From the official PixAI workflow guide, select Clone this template now under the Fated Pull section.

This opens the A Draw of Fate workspace, where you can view the original SSR-style result created with the template. To understand how the setup works, select View process and inspect the workflow behind the image.

The structure is fairly simple: the original character artwork is connected to another node that produces the finished gacha-style result.
Because the workspace initially opens in read-only mode, select Clone workspace in the upper-right corner. This creates your own editable copy while preserving the original workflow and its connections, giving you a version you can customize for Spider-Man.

## Step 2: Look at the Existing Workflow Before Changing Anything

Before replacing the original character, I first examined the cloned workflow to understand how its different parts worked together.

There are two main components: the source character image on the left and the editing step that transforms that image into the final SSR-style gacha screen.

When I selected the source image, its generation settings appeared, including the prompt, model, and other options used to create the original character. The second node used that character image as a reference and applied the instructions for generating the game-style reveal.
After looking through the setup, I realized there was no need to rebuild the workflow or add new nodes. The main change was simply to replace the original character with my Spider-Man artwork and let the existing connection carry it into the final editing stage.

## Step 3: Create the Spider-Man Image

With the workflow cloned, I moved to the source image node to replace the original character. Instead of creating the artwork in another tool and uploading it afterward, I generated the Spider-Man image directly inside PixAI Studio.

Select Tsubaki.3
I opened the model selector at the bottom-left of the image-generation node and switched the model to Tsubaki.3.
The cloned workflow originally had a LoRA attached that was incompatible with Tsubaki.3, so I removed it before generating the new character.

Generate the Spider-Man Artwork
For my first version, I wanted a recognizable Spider-Man design with a dynamic composition that would work well when passed through the gacha workflow. After testing the generation, I used a prompt featuring Spider-Man in his classic red-and-blue suit, crouching on a glass skyscraper ledge, with cinematic lighting, a detailed city background, and glowing blue energy effects.

The prompt I used was:
«“masterpiece, best quality, 1boy, Spider-Man, iconic red and blue suit, web pattern, dramatic action pose»

## Step 4: Replace the Original Character Content

Once the Spider-Man artwork was generated, I used it as the character input for the existing Fated Pull workflow. I didn’t need to add another node or modify the existing connections because the generated image was already passed from the source node into the editing node as its reference image.

I also kept the original SSR prompt in the editing node unchanged. It was already designed to transform the reference image into a social-game-style gacha screen, give the character an SSR presentation, generate a character name, and present the result as a newly revealed game unit.
This is one of the useful aspects of starting with a cloned template: most of the gacha-screen logic is already set up. My main task was simply replacing the original character with the Spider-Man artwork I had generated.

## Step 5: Adjust the Workflow for Your Spider-Man Version

I kept the adjustments to the cloned workflow fairly small rather than changing every part of the setup. The main changes were the character prompt, the generated Spider-Man artwork, and the model used for the final editing step.

After some testing, I switched the final generation model to PixAI Edit while keeping the existing SSR prompt unchanged. Because the Spider-Man artwork was already connected as the reference image, there was no need to rebuild the workflow or manually recreate the gacha effects.

This setup also made experimenting easier. If I wanted to try a different Spider-Man pose, background, or atmosphere, I could return to the Tsubaki.3 node, adjust the source prompt, generate another image, and pass the new result through the same SSR setup.
This made the workflow more flexible without requiring me to rebuild it each time.

## Step 6: Generate the Final Gacha Pull Screen

With the Spider-Man artwork connected as the reference image and PixAI Edit selected for the final editing stage, I ran the workflow.

The workflow transformed the source artwork into a complete game-style character reveal, adding the SSR presentation, interface elements, visual effects, and a generated character name around the original image.

The final result looked noticeably different from a standalone Spider-Man illustration. Instead, it had the visual structure of a character being revealed after a gacha pull. That was the main reason I used the Fated Pull workflow instead of trying to design the entire game interface manually.

My first few tests didn’t generate successfully, but after retrying the workflow, I was able to produce a working SSR result. This was also a useful reminder that individual generations can behave differently, so it’s worth trying again before changing a workflow that is otherwise set up correctly.

## Try 2 Spider-Man Variations

Once the first SSR screen worked, I didn’t need to clone another workspace to create a different version. I could simply reuse the same workflow, change the prompt in the Tsubaki.3 node, and generate a new source image.

### Classic Spider-Man SSR
For the first variation, I kept Spider-Man’s familiar red-and-blue appearance, combining it with a dramatic action pose, a city background, and bright lighting.

The result produced a colorful character reveal that felt similar to the splash art you might see when unlocking a new game unit.

### Spider-Man After Dark
For the second variation, I took Spider-Man in a darker direction. I changed the source prompt to place him on a rooftop at night, surrounded by city lights, rain, reflections, and more dramatic nighttime lighting.

I then passed the new Tsubaki.3 image through the same PixAI Edit setup without rebuilding the workflow. The resulting SSR screen maintained the gacha-style presentation while giving the character a noticeably darker atmosphere.
This was one of the main advantages of using the cloned Fated Pull template: once the workflow was set up, creating another variation was mostly a matter of changing the character idea and generating again.

## What I Learned from Using This Workflow

The biggest advantage of the Fated Pull workflow was that I didn’t have to figure out how to build a gacha screen from scratch. Once I cloned the workspace, the connection between the source character and the final editing step was already in place.

I also found that the source image plays an important role in the final result. Changing the pose, setting, and lighting in the Tsubaki.3 prompt could noticeably change the appearance of the finished SSR screen without requiring changes to the overall workflow.

Not every generation worked on the first attempt, either. I experienced a few failed generations while testing, but once the workflow was working, creating another Spider-Man variation was straightforward: change the source prompt, generate a new image, and run it through the same SSR setup.
For beginners, this makes cloning and adapting an existing workflow much easier than trying to understand and rebuild every node individually.

## I Also Joined a Spider-Man Community Contest on PixAI

After completing the SSR workflow, I explored more Spider-Man creations on PixAI and came across a community-hosted contest called “Spider Man: One Night Above the City.”

Because the contest focused on Spider-Man in a nighttime city setting, I decided to create a separate artwork specifically for the competition instead of reusing one of my gacha-screen results.

For my entry, I created a cinematic nighttime scene showing Spider-Man above an illuminated city. This gave me more freedom to focus on the atmosphere, skyline, lighting, and Spider-Man himself without the game UI from the Fated Pull workflow.
After generating a result I liked, I published the artwork and submitted it to the community contest.

## How Readers Can Join

If you want to create your own entry, start by opening the “Spider Man: One Night Above the City” contest page and checking the current theme and submission requirements.

Create an eligible Spider-Man artwork on PixAI and publish it publicly. Then return to the contest page, select Join Contest → Enter Now, choose your published artwork, and complete the submission process.

Before submitting, make sure to check PixAI’s contest participation guidelines and the live contest page, since eligibility and submission requirements may apply.

## Conclusion

Turning Spider-Man into a fictional limited SSR character was much easier with an existing PixAI Studio workflow than trying to build the entire gacha screen manually.

The process was straightforward: find Fated Pull in PixAI’s official workflow guide, clone the workspace, replace the original character with Spider-Man, select Tsubaki.3 for the source image generation, and run the result through the existing gacha setup.

Once the workflow was working, I could also create completely different Spider-Man variations simply by changing the source prompt instead of rebuilding the workspace.
If you want to try it yourself, clone Fated Pull and experiment with your own character or visual direction. And if you’re creating Spider-Man artwork, you can also take the concept beyond the gacha screen and explore the “Spider Man: One Night Above the City” community contest.

## Final Thoughts

What stood out to me most from this experiment was how much easier it can be to work with an existing AI workflow instead of building everything from scratch.

The Fated Pull template handled much of the structure needed for the gacha-style reveal, while I could focus on the creative side, generating Spider-Man artwork, experimenting with different prompts, and changing the mood through poses, backgrounds, and lighting.

It also showed the value of reusable workflows. Once the setup was working, creating new variations only required changing the source prompt and generating another image. There was no need to rebuild the entire workflow each time.
For anyone learning AI image workflows, this is a useful approach to try: start with an existing template, understand how its components connect, and then gradually adapt it to your own creative ideas.

