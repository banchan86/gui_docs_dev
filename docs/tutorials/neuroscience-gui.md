# Neuroscience GUI

The `Bonsai.GUI` package enables the creation of a comprehensive graphical user interface (GUI) for neuroscience Bonsai workflows. The following exercises will guide you through implementing several common UI elements, including:

- A button to start and stop experiments
- A text box for labeling files with an experimental or subject ID
- A mashup visualizer for overlaying an animal centroid on the raw video
- A chart for plotting extracted features from data streams
- A timer to show experiment runtime
- A property grid to adjust properties for operators (for instance, image threshold values for animal detection or number of trials for stimulus presentation)

In addition, we will cover how to arrange these UI elements into a cohesive layout and customize their properties.

Optional: We will also show you how to launch a GUI without the Bonsai Editor.

## Starter Workflow

For the purpose of this tutorial, we will start with a common neuroscience workflow that captures a video of a mice as well as its centroid. Implementing this workflow is beyond the scope of this tutorial but more information can be found in the [Acquisition and Tracking](https://bonsai-rx.org/docs/tutorials/acquisition.html) tutorial.

We will use a video of a foraging mouse that was generously provided by the Sainsbury Wellcome Centre Foraging Behaviour Working Group ((2023). Aeon: An open-source platform to study the neural basis of ethological behaviours over naturalistic timescales, https://doi.org/10.5281/zenodo.8413142). You can download the ForagingMouseExampleVid.avi video file here: https://doi.org/10.5281/zenodo.10629221. 

:::workflow
![Example](../workflows/neuroscience-starter-workflow.bonsai)
:::

To replicate this workflow:
- Save the video to a folder. 
- Copy the workflow in this container by clicking on the copy button on the top right
- Paste it in the Bonsai editor.
- Save the workflow in the same folder where the video is saved. 
- Run the workflow once to make sure that it runs correctly and that you have the required packages installed. A copy of the video file as well as a csv file containing the centroid of the mice should be produced in the same folder.
- Double-click on any of the nodes to visualize the data stream/transformation that it is processing.

> [!NOTE]
> If any of the operators appear with a cross hatch pattern, search for the missing package in the Bonsai package manager and install it.

> [!NOTE]
> For this tutorial, we have used a `FileCapture` operator to playback the file, but you can replace it with any live streaming video source like `CameraCapture` for your real experiments.






