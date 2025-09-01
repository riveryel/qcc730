This nvm is generated from below
1) source code

https://docs.qualcomm.com/bundle/publicresource/topics/RNO-250508055332/ReleaseNote.html
repo init -u https://git.codelinaro.org/clo/le/le/product/manifest.git -b release -m AU_LINUX_EMBEDDED_IOT.FM.1.0.R1_TARGET_ALL.01.09.038.xml --repo-url=https://git.codelinaro.org/clo/tools/repo.git --repo-branch=aosp-new/stable

3) env setup guide

https://docs.qualcomm.com/bundle/publicresource/topics/80-Y8730-1/development_environment_setup.html

4) document guide for nvm package

https://docs.qualcomm.com/bundle/publicresource/topics/80-Y8730-2/qcc730_nvm_programmer.html

5) Key - notice

Generate "nvm_programmer.exe" by below options:

a) Merge binary on Windows by "copy /b nvm_programmeraa + nvm_programmerab nvm_programmer.exe"

b) Merge binary on Linux by "cat nvm_programmeraa nvm_programmerab > nvm_programmer.exe"


