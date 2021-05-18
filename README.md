---
title: VS Code Remote Development
date: 18/05/2021 
author:
 - Bhawick Jain
or: 20210518073902
---

Having jupyter notebooks with its various kernels is great. But what if you just want to run and debug a simple script? You'd need a code editor, sure, but exactly do you debug the code if it is inside a container? I deally I would like to be able to add breakpoint and do all the various debugging exercises I usually do. Enter VS Code Remote. 

`[x]` Python IDE setup  
`[ ]` Check [[vsc-python](https://code.visualstudio.com/docs/python/python-tutorial)] to see if any setup has been missed  
`[ ]` C++ Remote IDE Setup using [[vsc-cpp](https://code.visualstudio.com/docs/cpp/introvideos-cpp)]  
`[ ]` Develop procedure for production [[vsc-advconfig](https://code.visualstudio.com/docs/remote/containers-advanced)] may help withi this.  

`[?]` What does the port forwarding option do in the `.devcontainer/devcontainer.json` file.  
`[?]` Is `devcontainer.json` trying to be another yet another dockerfile?  

`[?]` VS Code uses the old `docker-compose` command, will it move to `docker compose` soon?  
`>>>` Likely once it is out of preview.  

You can also work directory off a repo, eliminating any need to mounted volumes.

### Usage

```bash
code .
```

You will be prompted in bottom left corner that VS Code has detected a `.devcontainer` folder will ask you want to jump starting. Click `Reopen in Container`. Otherwise `Remote-Containers: Rebuild and Reopen in Container` with VS Code's command menu (`cmd + shift + p`).

### References

[[vsc-remote](https://code.visualstudio.com/docs/remote/remote-overview)] VS Code Remote Development — VS Code Docs  
[[vsc-running](https://code.visualstudio.com/docs/remote/attach-container)] Attach to a running container — VS Code Docs  
[[vsc-python](https://code.visualstudio.com/docs/python/python-tutorial)] VS Code intro to Python — VS Code Docs  
[[vsc-cpp](https://code.visualstudio.com/docs/cpp/introvideos-cpp)] VS Code Intro to Python — VS Code Docs  
[[vsc-advconfig](https://code.visualstudio.com/docs/remote/containers-advanced)] Advanced Container Configuration — VS Code  
[[vs-ext-remotedev](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)] Remote Development — (Visual Studio Code Extension Packs)  
