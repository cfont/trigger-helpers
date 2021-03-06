# trigger-helpers
Provides a step debugger in the php runtime with xdebug and some functions commonly used in workflow trigger development.
Can be used to speed up development of workflow triggers by providing code completion for ee functions and  allowing the designer
to inspect results from ee function calls and see the exact data structures returned.

Also provides working examples of use PHP curl commands to interact with Ethos APIs.

Steps to use

1. Download and install git, visual studio code, and docker desktop if needed.
   1. https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
   2. https://code.visualstudio.com/download
   3. https://www.docker.com/products/docker-desktop
2. In VS code add ['Remote - Containers' extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
3. From command prompt at the location of your preferred working directory clone the repository

   ```
   git clone https://github.com/eli-hickey/trigger-helpers.git
   ```

4. In VS Code use command pallet command 'Remote-Containers: Open Folder in Container...' and select the trigger-helpers folder created by the git clone command.
6. Rename /project/scripts/setup/env.example to .env and add your api key and region to it (US  = 'com', Canada = 'ca' ...)
7. Run the Demo ethosExamples to verify everything is working
   1. Open the /scripts/examples/ethosExamples.php
   2. Add a breakpoint on the last line
   3. Run (f5)



You are now ready to get your ethos data with some ee functions.

To refresh the provided functions periodically run git pull