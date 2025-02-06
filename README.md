# Sionna for Networked Robotics

This codebase facilitates the simulation of Ray Tracing and Propagation using SIONNA for secure and mapless robot navigation.

## Introduction

This experiment introduces a novel testbed designed for privacy-preserving robot navigation, utilizing the Sionna RT and Blender tools. The testbed addresses growing privacy concerns associated with sensing data in autonomous systems, presenting a differential raytracing approach for precise sensitivity analysis in unstructured environments.

## Setup and Prerequisites

### Prerequisites

Before setting up the privacy-preserving robot navigation testbed, ensure you have the following prerequisites installed:

- Ubuntu OS
- Sionna - [Download](https://github.com/NVlabs/sionna)
- Blender LTS vs 3.6.12 - [Download](https://www.blender.org/download/lts/3-6/)
- Mitsuba 3 - [Download](https://www.mitsuba-renderer.org/)
- Jupyter Notebook - [Installation Guide](https://jupyter.org/install)

### Getting Started

Once you have successfully installed all the necessary dependencies, proceed to run the notebook. Replace the default scene with custom scenes that you've created using Blender and exported as `.xml` files with Mitsuba. This step allows you to tailor the simulation to your specific environments, ensuring accurate and personalized results in the simulation process. Simply follow the instructions in the notebook to seamlessly integrate your customized scenes and enhance the overall simulation experience.

### Instructions

1. The key element of this simulation is the *scene* used by this notebook. Start by either creating from scratch or using the example scenes provided by sionna here in [SIONNA RT Documentation](https://nvlabs.github.io/sionna/api/rt.html).

2. Export the scene using Mitsuba Renderer as a .xml file.

3. Replace the file_path for scene.load().

4. Run each cell to visualize the outcome.

5. Adjust parameters like num_samples, max_depth, transmitter(position=), and receiver(position=) to tailor the simulation results according to the specifics of your scene. Fine-tune these parameters to achieve outcomes that align with the characteristics of your particular environment.

## FAQ

- *Q: How to resolve "llvm not found error"?*
  - A: It's probably a name error, so try finding the llvm file and renaming it!

- *Q: Can I integrate this simulation with robotic control algorithms?*
  - A: Yes, the simulation results can be used to inform and validate mapless navigation algorithms for robotic systems.


## Cite

If you find this simulation framework useful in your research, please cite our work:

Amatare, Sunday and Singh, Gaurav and Samson, Michelle and Roy, Debashri, RagNAR: Ray-tracing based Navigation for Autonomous Robot in Unstructured Environment (April 30, 2024). Available at SSRN: https://ssrn.com/abstract=4915850 or http://dx.doi.org/10.2139/ssrn.4915850

## Acknowledgments

Thank you for choosing the privacy-preserving robot navigation testbed. For any questions, feedback, or collaboration opportunities, please feel free to reach out.



