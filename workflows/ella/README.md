# ComfyUI Workflow collection

[Go back to overview](../README.md)

## ELLA

Comparison workflow and example results with [ELLA (Equip Diffusion Models with LLM for Enhanced Semantic Alignment)](https://github.com/TencentQQGYLab/ELLA)

## Guide

Using [this node](https://github.com/ExponentialML/ComfyUI_ELLA) we can use conditioning through ELLA, but we can also combine the conditioning with regular checkpoints. SDXL (Juggernaut v9) added for another comparison (this one will not use ELLA as SDXL will not be released for ELLA).

The prompts are focused on testing the prompt adherence. The goal is to get the subjects from the prompt but as well as the correct subject colors (for example a red hat, a blue suit, etc). Take a look at the comparison table images to see the differences in colors, subjects, context bleed, etc.

Try out the workflow as well if you want to make your own comparisons, use the toggles to enable/disable different plots, and optionally you can enable/disable the plot, high-res script or a lora stacker for both SD15(ELLA or Default)/SDXL.

### Color prompt comparison example

Comparison table images of ELLA/Combined/SD15/SDXL

`closeup of a grey cat wearing a blue suit, a red hat and a green tie is sitting on a white table in a room with big windows viewing over a desert landscape covered by flowers`

| ELLA | Combined |
| --- | --- |
| [<img src="/workflows/ella/comparison/grey-cat/ella_thumb.png" />](/workflows/ella/comparison/grey-cat/ella.png) | [<img src="/workflows/ella/comparison/grey-cat/combined_thumb.png" />](/workflows/ella/comparison/grey-cat/combined.png) |

| SD15 | SDXL |
| --- | --- |
| [<img src="/workflows/ella/comparison/grey-cat/sd15_thumb.png" />](/workflows/ella/comparison/grey-cat/sd15.png) | [<img src="/workflows/ella/comparison/grey-cat/sdxl_thumb.png" />](/workflows/ella/comparison/grey-cat/sdxl.png) |

Extra comparisons:

| SD3 | Dall-E |
| --- | --- |
| [<img src="/workflows/ella/comparison/grey-cat/sd3_thumb.webp" />](/workflows/ella/comparison/grey-cat/sd3.webp) | [<img src="/workflows/ella/comparison/grey-cat/dalle_thumb.webp" />](/workflows/ella/comparison/grey-cat/dalle.webp) |

| Midjourney v5 | Midjourney v6 |
| --- | --- |
| [<img src="/workflows/ella/comparison/grey-cat/midjourney5.png" />](/workflows/ella/comparison/grey-cat/midjourney5.png) | [<img src="/workflows/ella/comparison/grey-cat/midjourney6.png" />](/workflows/ella/comparison/grey-cat/midjourney6.png) |

`Closeup of a white cat wearing a brown suit, a purple hat, and a red tie, sitting on a green table in a room with big windows viewing over a desert ocean covered by yellow boats`

| ELLA | Combined |
| --- | --- |
| [<img src="/workflows/ella/comparison/grey-cat/ella2_thumb.png" />](/workflows/ella/comparison/grey-cat/ella2.png) | [<img src="/workflows/ella/comparison/grey-cat/combined2_thumb.png" />](/workflows/ella/comparison/grey-cat/combined2.png) |

| SD15 | SDXL |
| --- | --- |
| [<img src="/workflows/ella/comparison/grey-cat/sd152_thumb.png" />](/workflows/ella/comparison/grey-cat/sd152.png) | [<img src="/workflows/ella/comparison/grey-cat/sdxl2_thumb.png" />](/workflows/ella/comparison/grey-cat/sdxl2.png) |

## Conclusion

There seems to be improvement in these prompt tests, but there are also prompt cases that give no advantage at all. The combined conditioning between ELLA and SD15 seem to be interesting as it (in some cases) can improve prompt adherence without losing too much of the original checkpoint style.

## Workflow

This workflow includes the metadata, you can also download the workflow.json in this directory.

![Workflow](/workflows/ella/workflow.png)

## Notes

- The SD3 example was provided via https://www.reddit.com/r/StableDiffusion/comments/1c78ltj/comment/l06bome/
