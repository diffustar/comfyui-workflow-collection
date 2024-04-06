# ComfyUI Workflow collection

[Go back to overview](../README.md)

## SAL-VTON clothing swap

A rough example implementation of the [Comfyui-SAL-VTON](https://github.com/ratulrafsan/Comfyui-SAL-VTON) clothing swap node by ratulrafsan. Take a look at the linked repository for more information and requirements of the input images and example inputs.

![Workflow](/workflows/sal-vton-clothing-swap/workflow.png)

## Guide

You can use any input checkpoint or image, but make sure to follow the requirements of the [Comfyui-SAL-VTON](https://github.com/ratulrafsan/Comfyui-SAL-VTON) repository. 

This workflow will use the RemBG nodes to remove the background of the input images and to create a mask for the person/garment. Afterwards the mask is reused to cut out the result of the SAL-VTON node and to paste it onto the original image. 

The output is quite dependent on the original clothing and the provided clothing. When the clothing is too different the result might not look as expected or overlap/holes might appear on the result because the mask is not perfectly fitting the person/garment.

## Reference images

Generated input image: (original image)

![Generated input image](/workflows/sal-vton-clothing-swap/example-input.png)

Generated output image A: (SAL-VTON result)

![Generated output image A](/workflows/sal-vton-clothing-swap/example-output-a.png)

Generated output image B (pasted result on original image)

![Generated output image B](/workflows/sal-vton-clothing-swap/example-output-b.png)
