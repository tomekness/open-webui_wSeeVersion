# Customized Open Web UI

This project is a customized fork of the original [Open Web UI](https://github.com/open-webui/open-webui). 

## Acknowledgments
Open Web UI is a powerful open-source project. This fork builds upon their hard work to meet specific needs and extended control functionalities. The original project is available at https://github.com/open-webui/open-webui.

## Purpose of the Fork
This fork is just a workaround for setting customized (but unfortunately hard-coded) default model parameters for all users. Otherwise, new users start with unsuitable and disadvantageous model parameters. 

Furthermore, different users with varying parameters would repeatedly cause the language model to drop and reload, resulting in a very unresponsive chat interface.

It retains compatibility with updates from the main Open Web UI project wherever possible.

### changes

- Default Model parameters are hardcoded in 
src/lib/components/chat/Settings/Advanced/AdvancedParams.svelte

Values we adjusted:
Size of context window,  --> num_ctx
Temperature --> temperature 


- To disable the save-button and prevent users to change the model parameters go do 
src/lib/components/chat/Settings/General.svelte

