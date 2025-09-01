This "nvm_programmer.exe" is packaged from steps

1) Get source code

https://docs.qualcomm.com/bundle/publicresource/topics/RNO-250508055332/ReleaseNote.html

repo init -u https://git.codelinaro.org/clo/le/le/product/manifest.git -b release -m AU_LINUX_EMBEDDED_IOT.FM.1.0.R1_TARGET_ALL.01.09.038.xml --repo-url=https://git.codelinaro.org/clo/tools/repo.git --repo-branch=aosp-new/stable

3) Env setup guide

https://docs.qualcomm.com/bundle/publicresource/topics/80-Y8730-1/development_environment_setup.html

4) Document guide for nvm package

https://docs.qualcomm.com/bundle/publicresource/topics/80-Y8730-2/qcc730_nvm_programmer.html


Generate "nvm_programmer.exe" by below options:

1) On Windows, merge binary: "copy /b nvm_programmeraa + nvm_programmerab nvm_programmer.exe"

2) On Linux, merge binary: "cat nvm_programmeraa nvm_programmerab > nvm_programmer.exe"


Usage of "nvm_programmer.exe"

1) Command: "nvm_programmer.exe -s ch347 -i <FERMION_NVM_PROGRAMMER.elf> sub_cmds"

Usage samples
1) "nvm_programmer.exe -s ch347 -i <FERMION_NVM_PROGRAMMER.elf> --nvm-name rram -b 0x20A400 -f <FERMION_SBL_HASHED.elf>"
2) "nvm_programmer.exe -s ch347 -i <FERMION_NVM_PROGRAMMER.elf> --nvm-name rram -b 0x21A400 -f <FERMION_IOE_QCLI_DEMO.bin>"
3) "nvm_programmer.exe -s ch347 -i <FERMION_NVM_PROGRAMMER.elf> --reset"

