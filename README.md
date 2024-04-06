# ComfyUI Workflow collection

While experimenting with ComyUI I'll share some of the workflows in this repository. 
In the workflows directory you will find a separate directory containing a `README.md` file with a description of the workflow and a `workflow.png`/`workflow.json` which you can both drop into ComfyUI to import the workflow.

## Running workflows

To run a workflow, download the `workflow.json` or `workflow.png` file and import it into ComfyUI. If you are missing custom nodes ComfyUI will throw an error. Using the ComfyUI Manager plugin you can install the missing nodes. Afterwards restart ComfyUI and reload the workflow.

## Workflows

### XYZ Plot

A simple example workflow to make a XYZ plot using the plot script combined with multiple KSampler nodes.

[Read more](/workflows/xyz-plot/README.md)

Workflow preview: (this image does not contain the workflow metadata !)

![Workflow](/assets/preview-xyz-plot.png)

### SAL-VTON clothing swap

A rough example implementation of the [Comfyui-SAL-VTON](https://github.com/ratulrafsan/Comfyui-SAL-VTON) clothing swap node by ratulrafsan.

[Read more](/workflows/sal-vton-clothing-swap/README.md)

Workflow preview: (this image does not contain the workflow metadata !)

![Workflow](/assets/preview-sal-vton-clothing-swap.png)
