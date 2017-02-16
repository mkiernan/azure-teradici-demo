# Deploy a Windows NV VM.
# **WIP**
* [Prereqs](#prereqs)
* [MSFT OSCC](#msft-oscc)
* [Reporting Bugs](#reporting-bugs)
* [Patches and pull requests](#patches-and-pull-requests)

#### Prereqs
**Obtain a Trial License For the Windows Graphics Agent from [here](http://connect.teradici.com/cas-trial) to put in the template parameter**

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-accessplatform-windows-gpu%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-accessplatform-windows-gpu%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>
* PCoIP Client Download for Windows is [here](http://teradici.com/swclient-windows)
* nView needs to be enabled manually. [User Guide](http://www.nvidia.com/content/quadro/pdf/nView-user-guide.pdf)
* Collection of the user dumps for the NVIDIA Display Driver 369.71  from within the VM on Display Driver Crash if occurs.
 * Details are [here](http://nvidia.custhelp.com/app/answers/detail/a_id/3335/~/tdr-(timeout-detection-and-recovery)-and-collecting-dump-files) 
* PCoIP RC Agent Log Collection (2.7.0.3589 ) or (2.7.0.4060) from the Teradici System Tray (right click Teradici Icon on System Tray) and collect Agent Logs (from the pop-up).
 * PCoIP RC Agent 2.7.0.4060 uses Multiple PCoIP encoding and options are there during provisioning to use either (2.7.0.4060 or 2.7.0.3589). The logic is present in the Script extension.
* The PCOIP Agent Logs (v1.9.*) from the Office Client machine of the end-user from <code>C:\Users<user_name>\AppData\Local\Teradici\PCoIPClient\logs</code>

#### MSFT OSCC
This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

#### Reporting bugs

Please report bugs  by opening an issue in the [GitHub Issue Tracker](https://github.com/Azure/azure-accessplatform-windows-gpu/issues)

#### Patches and pull requests

Patches can be submitted as GitHub pull requests. If using GitHub please make sure your branch applies to the current master as a 'fast forward' merge (i.e. without creating a merge commit). Use the `git rebase` command to update your branch to the current master if necessary.


